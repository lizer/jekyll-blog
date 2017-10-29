---
layout: post
title: discussion with ZB
date: '2017-10-28 17:06:13 +0000'
categories: jekyll update
published: true
--- 

<script type="text/javascript"
	src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS_HTML,
	/javascripts/MathJaxLocal.js
">
</script>

### property
If, for $$\alpha \geq {1}/{8},$$
\\[
E  \{ F(x^{(s)}) - F(x)  \} \leq (1+\alpha)^{-s} \epsilon_0. 
\\]
Then it imples that  
\\[
E \{ F(x^{(s)}) - F(x) \} \leq \epsilon,
\\]
if $$s = C (1+1/\alpha) \log ({\epsilon_0}/{\epsilon}).$$ 


### proof
If
\\[
s \geq \{ {1}/{\log(1+\alpha)} \} \log (\epsilon_0 / \epsilon), 
\\]
we have
\\[
E  \{ F(x^{(s)}) - F(x) \} \leq (1+\alpha)^{-s} \epsilon_0 \leq \epsilon. 
\\]


Thus, we have to proof that for some $$C$$ and $$\alpha > 1/ 8$$
\\[
C (1+1/\alpha) \log (\epsilon_0 / \epsilon) \geq \{ 1 / \log(1+\alpha)) \log (\epsilon_0 / \epsilon)
\\]


Equavelenlly, for some $$C$$ and $$\alpha > 1/ 8$$
\\[
C (1 + \alpha) / \alpha  \geq  1 / \log(1+\alpha).
\\]

Consider, 
\\[
f(\alpha) :=  \frac{(1+\alpha) \log(1+\alpha)}{\alpha}.
\\]
We want that 
\\[
f(\alpha) \geq 1/C.
\\]
Since $$f(\alpha)$$ is an ascend function. Then, if we let $$C = f(1/8)$$, we have that 
\\[
f(\alpha) \geq 1/C,
\\]
for $$\alpha \geq 1/8.$$

