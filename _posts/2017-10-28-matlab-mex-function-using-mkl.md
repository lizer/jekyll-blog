---
layout: post
title: Matlab mex function using Intel MKL BLAS
date: '2017-10-28 17:05:13 +0000'
categories: jekyll update
published: true
--- 

### 使用的代码
'''c++
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
'''
### 错误：

### 参考文献：
[A New Linking Model- SDL mkl_rt Since Intel MKL 10.3](https://software.intel.com/en-us/articles/a-new-linking-model-single-dynamic-library-mkl_rt-since-intel-mkl-103/)

### 正确的编译：

