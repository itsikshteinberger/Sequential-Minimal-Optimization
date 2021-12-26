# Sequential Minimal Optimization algorithm (SMO)


![](https://images.pexels.com/photos/355948/pexels-photo-355948.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=1000)

<br/>

<h3 align="center">
  Implementing the SMO algorithm from scratch
</h3>

<p align="center">
  <br/> Sequential Minimal Optimizatiom algorithm <a href="https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/tr-98-14.pdf">[1]</a> is a faster algorithm for training support vector machines designed by J. C. Platt. <br/>
</p>

<p align="center">
Training a support vector machine requires the solution of a very large quadratic programming (QP) optimization problem. <br/>
SMO breaks this large QP problem into a series of smallest possible QP problems. <br/>
These small QP problems are solved analytically, which avoids using a time-consuming numerical QP optimization as an
inner loop. <br/>
The amount of memory required for SMO is linear in the training set size, which allows SMO to handle very large training sets. <br/> 
Because matrix computation is avoided, SMO scales somewhere between linear and quadratic in the training set size for various test problems, while the standard chunking SVM algorithm scales somewhere between linear and cubic in the training set size. <br/>
SMO’s computation time is dominated by SVM evaluation, hence SMO is fastest for linear SVMs and sparse data sets. <br/> 
On realworld sparse data sets, SMO can be more than 1000 times faster than the chunking algorithm. <br/>
</p>

 <br/>

### References:

[1] [Sequential Minimal Optimization: A Fast Algorithm for Training Support Vector Machines, 1998](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/tr-98-14.pdf).
