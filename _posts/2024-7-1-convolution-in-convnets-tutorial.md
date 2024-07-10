---
layout: post
title:  "Convolution in ConvNets Tutorial"
date: 2024-7-1
image: assets/images/conv.png
tags: [ AI, tutorials, resources, summer2024 ]
---

In ConvNets, convolution refers to the process of applying a filter or a kernel to an input or feature map.

Convolution is a common image-processing technique that changes the value of a pixel according to the values of its surrounding pixels. Many common image filters, such as blurring, detecting edges, sharpening, and embossing, derive from convolution.

Kernels form the basis of convolution operations. Kernels are arrays or matrices of weights that indicate the influence of a pixel’s neighbors on its final value. To calculate the value of each transformed pixel, a convolution operation adds the products of each surrounding pixel value with the corresponding kernel value. During a convolution operation, the kernel passes over every pixel in the image, repeating this procedure, and then applies the effect to the entire image.  

**Input image (7x7x3)**   

x[:, :, 0]     
<img src="/assets/images/r.png" class="img-fluid" />
   

x[:, :, 1]     
<img src="/assets/images/g.png" class="img-fluid" />


x[:, :, 2]     
<img src="/assets/images/b.png" class="img-fluid" />


**Filter W0 (3x3x3)**   

w0[:, :, 0]   
<img src="/assets/images/f0_r.png" class="img-fluid" />

w0[:, :, 1]   
<img src="/assets/images/f0_g.png" class="img-fluid" />

w0[:, :, 2]   
<img src="/assets/images/f0_b.png" class="img-fluid" />

**Filter W1 (3x3x3)**   

w1[:, :, 0]   
<img src="/assets/images/f1_r.png" class="img-fluid" />

w1[:, :, 1]   
<img src="/assets/images/f1_g.png" class="img-fluid" />

w1[:, :, 2]   
<img src="/assets/images/f1_b.png" class="img-fluid" />

**Bias b0 (1x1x1)**   
b0[:, :, 0]   
1   

**Bias b1 (1x1x1)**   
b1[:, :, 1]   
0   

**Output feature map (3x3x2)**   
The size of the output feature map is determined by several factors including the size of the input or feature map, the size of the filter, and the stride of the convolution operation.

output[:, :, 0]   
<img src="/assets/images/o0.png" class="img-fluid" />

output[:, :, 1]   
<img src="/assets/images/o1.png" class="img-fluid" />


