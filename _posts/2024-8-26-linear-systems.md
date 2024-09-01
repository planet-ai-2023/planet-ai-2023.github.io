---
layout: post
title:  "Linear Systems"
date: 2024-8-26
image: assets/images/ls.png
tags: [ planet, AI, tutorials, resources ]
---

A system of linear equations, or a linear system, is a collection of one or more linear equations involving the same variables. An example is   
2x<sub>1</sub> - x<sub>2</sub> = 0   
x<sub>1</sub> + x<sub>2</sub> = 3   
The solution of the system of the above two equations in two variables is easy- it amounts to finding the intersection of two lines.   

The essential information of a linear system can be recorded compactly in a rectangle array called a matrix. Given the above system wiht the coefficients of each variable aligned in columns, the matrix <code>sympy.Matrix([[2, -1], [1, 1]])</code> is called the coefficient matrix or matrix of coefficients of the system. And the matrix <code>sympy.Matrix([[2, -1, 0], [1, 1, 3]])</code> is called the augmented matrix of the system. An augmented matrix of a system consists of the coefficient matrix with an added column containing the constants from the respective right sides of the equations.


<br/>
<br/>
<script src="https://gist.github.com/planet-ai-2023/b1656d62d35c7ce6ef7f141a105858a3.js"></script>
<br/>
<br/>
