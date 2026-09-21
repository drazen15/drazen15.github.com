---
layout: post
title: 浮点数入门
date: 2013-03-19 21:34
comments: true
tags:
- Code
- Floating Point
- Python
categories: Code
---
在[《learn python the hard way》](http://learnpythonthehardway.org/)的第三章中遇到了浮点数的概念。Google了一下，作为浮点数的入门

### 什么是浮点数

相对于定点数(常用来表示整数和纯小数,如:`8`,`0.6`等等),浮点数能够表示带小数部分的数字(如:`12.34`,`939001.32`,`0.00023`,`8.0`等).  
定点数的缺点在于其形式过于僵硬,固定的小数点位置决定了固定位数的整数部分和小数部分,不利于同时表达特别大或者特别小的数字.而浮点数很好的解决了这一问题,计算机将浮点数分成两部分存储,一部分表示值,另一部分用于对值进行放大或者缩小.因此浮点数可以表示小数值,非常大和非常小的数值.

### 浮点数的表示方法

C++中浮点数有两种表示方法:

**标准小数点表示法**

	12.34			//floating-point
	939001.32		//floating-point       
	0.00023			//floating-point
	8.0				//floating-point

**E表示法**

3.45E6是一个用E表示法表示的浮点数,这指的是3.45与1000000相乘的结果;E6指的是10的6次方,因此3.45E6表示的是3450000,6被称为指数,3.45被称为尾数.E表示法确保数字以浮点格式存储,数字中没有空格,指数可以是整数也可以是负数,浮点数也可以为负数.

	2.52e+8				//can use E or e, + is optional
    8.33E-4	 			//exponent can be negative
    7E5					//same as 7.0E+05
    -18.32e`13			//can have + or - sign in front
    7.123e12 			//US public debt, early 2004
    5.98E24 			//mass of earth in kilograms

目前对于浮点数就了解这么多,再深入的关于浮点数的精度,与二进制的转换,浮点类型等,后面接触到的话再继续学习.