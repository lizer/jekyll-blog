---
layout: post
title: Matlab mex function using Intel MKL BLAS
date: '2017-10-28 17:05:13 +0000'
categories: jekyll update
published: true
--- 

### 1.使用的代码:

```
#include "mex.h"
#include "mkl.h"

void mexFunction(int nlhs, mxArray *plhs[], 
    int nrhs, const mxArray *prhs[])
{
	double  a = *mxGetPr(prhs[0]);
	size_t  n =  mxGetM (prhs[1]);
	double* x =  mxGetPr(prhs[1]);
	double* y =  mxGetPr(prhs[2]);
    
	plhs[0]= mxCreateDoubleMatrix(1,1,mxREAL);
	double* z=mxGetPr(plhs[0]);        

	if (n!=mxGetM(prhs[2])){
	 	mexPrintf("x and y have different sizes.\n");
		return;
	}

	*z = cblas_ddot(n, x, 1, y, 1);

	mexPrintf("We finish the work!\n");
	return;
}
```

### 2.错误:
#### 编译方法:

```
>>mex mklabc.c -I/$(MKL_INCLUDE_DIR) -L$(MKL_LIB_DIR) -lmkl_rt -lgomp -lmkl_intel_lp64 -lmkl_gnu_thread -lmkl_core -lgomp
```

编译成功。但是，运行会有大问题。。。

#### 测试:

```
>> a = 1

a =

1

>> b = 2

b =

2

>> c = 4

c =

4

>> mklabc(a, b, c)
```

运行后，matlab 崩溃，错误信息如下：

```
Intel MKL FATAL ERROR: Cannot load libmkl_avx2.so or libmkl_def.so.
```


### 3.参考文献：
[A New Linking Model- SDL mkl_rt Since Intel MKL 10.3](https://software.intel.com/en-us/articles/a-new-linking-model-single-dynamic-library-mkl_rt-since-intel-mkl-103/)


### 4.修正：
#### 编译方法:

```
>>mex -v mklabc.c -I/$(MKL_INCLUDE_DIR) -L$(MKL_LIB_DIR) -lmkl_rt -lgomp
```

#### 测试:

```
>> a = 1

a =

     1

>> b = 2

b =

     2

>> c = 4

c =

     4

>> mklabc(a, b, c)
We finish the work!

ans =

     8
>> 
```

**The end**.
