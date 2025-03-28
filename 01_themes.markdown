---
layout: page
title: Highlights
permalink: /highlights/
---

### Optimal Regularizers for a Data Source

<img src="/assets/images/Ex1.png" alt="Reg_Ex1" width="180"/> <img src="/assets/images/Ex2.png" alt="Reg_Ex1" width="180"/> <img src="/assets/images/Ex3.png" alt="Reg_Ex1" width="180"/> <img src="/assets/images/Ex4.png" alt="Reg_Ex1" width="180"/>

Regularizers are penalty functions that are frequently deployed in the context of solving inverse problems.  These play an important role of addressing ill-posedness that might arise because of a lack of data, for instance.  To give an illustration, if we believe that our data is well approximated as a sparse vector, then a reasonable choice of regularizer to apply is the L1-norm.

Regularization techniques are extremely powerful in practice -- the difficulty of deploying such techniques is that we frequently do not know the appropriate choice of regularizer.  In this line of work, we ask

> Given a data source, can we identify the _optimal_ choice of a regularization function for use, say, on a downstream task?  How do we formulate such a conceptual problem into a mathematical question that is meaningful to us?  How do _computational_ _considerations_ affect our preference for certain families of regularizers over others?

1. Optimal Convex and Nonconvex Regularizers for a Data Source, <a href ="https://www.oscarleong.com/">O. Leong</a>, <a href ="https://sites.google.com/view/eliza-oreilly/home">E. O'Reilly</a>, Y. S. Soh, and [V. Chandrasekaran](http://users.cms.caltech.edu/~venkatc/), *Foundations of Computational Mathematics (accepted)*, Dec '22, <a href = "https://arxiv.org/abs/2212.13597">[arXiv]</a>

1. The Star Geometry of Critic-Based Regularizer Learning, <a href ="https://www.oscarleong.com/">O. Leong</a>, <a href ="https://sites.google.com/view/eliza-oreilly/home">E. O'Reilly</a>, Y. S. Soh, *NeurIPS*, Sep '24, <a href = "https://arxiv.org/abs/2408.16852">[arXiv]</a>


### Graph Matching, Gromov-Wasserstein

<img src="/assets/images/gwsdp_matching.png" alt="Matching" width="340"/> <img src="/assets/images/gwsdp_support.png" alt="Transportation Map Support" width="340"/> <img src="/assets/images/gwsdp_elephant.png" alt="Computer Vision Example" width="300"/> <img src="/assets/images/gwsdp_noisygraphs.png" alt="Computer Vision Example" width="150"/>

1. Sum-of-Squares Hierarchy for the Gromov-Wasserstein Problem, HA Tran, BT Nguyen, YS Soh, *pre-print*, Feb '25 <a href = "https://arxiv.org/abs/2502.09102">[arXiv]</a>

1. Exactness Conditions for Semidefinite Relaxations of the Quadratic Assignment Problem, J. Chen, Y. S. Soh, *pre-print*, Sep '24 <a href = "https://arxiv.org/abs/2409.08802">[arXiv]</a>

1. Semidefinite Relaxations of the Gromov-Wasserstein Distance, J. Chen, B. T. Nguyen, Y. S. Soh, *NeurIPS '24*, Dec '23, <a href = "https://arxiv.org/pdf/2312.14572">[arXiv]</a>

1. The Lovasz Theta Function for Recovering Planted Clique Covers and Graph Colorings, J. Hou, Y. S. Soh, <a href ="https://sites.google.com/site/antoniosvarvitsiotis/">A. Varvitsiotis</a>, *pre-print*, Oct '23, <a href = "https://arxiv.org/abs/2310.00257">[arXiv]</a>


### Learning Data Representations with Symmetries

Suppose we want to learn a data representation for an image processing task.  Ideally, the representation should be invariant to translations and rotations -- after all, natural images still look like images after rotations!  The basic question this line of work investigates is:

> How do we learn data representations that incorporate these invariances in a principled manner?  

> Given a generic group, can I provide a general _recipe_ that allows me to learn a data representation that respect these invariances automatically?

1. Dictionary Learning under Symmetries via Group Representations, <a href ="https://subhro-ghosh.github.io/">S. Ghosh</a>, A. Y. R. Low, Y. S. Soh, Z. Feng, B. K. Y. Tan, *pre-print*, Jun '23, <a href = "https://arxiv.org/abs/2305.19557">[arXiv]</a>

1. Group Invariant Dictionary Learning, Y. S. Soh, *Transactions on Signal Processing*, Jun '21, <a href = "https://ieeexplore.ieee.org/document/9461688">[Article]</a> <a href = "https://arxiv.org/abs/2007.07550">[arXiv]</a> <a href = "https://github.com/bkytan/gidl">[Code] (maintained by Brendan KY Tan)</a>



### Fitting Convex Sets to Data

<img src="/assets/images/Exp_F1b_s00_LS_n200.png" alt="Least Squares Estimate of Sphere" width="180"/> <img src="/assets/images/Exp_F1b_s00_AMsd_n200.png" alt="SDP Description of Sphere" width="180"/> <img src="/assets/images/Exp_3D_Lung_LS_n300.png" alt="Least Square Estimate of Lung" width="140"/> <img src="/assets/images/Exp_3D_Lung_q6_n300.png" alt="SDP Description of Sphere with 6x6 matrix" width="140"/>

> Given a collection of data-points in space, how do we fit a convex set or model to these points?

Firstly, why should we care?  It turns out that a number of data processing problems can actually be viewed as the geometric task of fitting a convex set to data!  Consider, for instance, the task of learning a _regularizer_ for data-processing.  For concreteness, we restrict to regularizers that are expressible via _Linear_ _Programming_.  It turns out that this process is known as _dictionary_ _learning_ or _sparse_ _coding_ in the literature.

Some of the key questions we ask: 

> What computational or data processing task can be viewed via a geometric lens as one of fitting a convex set to data? 

> How should we parameterize the convex set?  

As it turns out, if we restrict to convex sets that are expressible via Linear Programs, we recover a number of existing methods (dictionary learning, sparse coding, non-negative matrix factorization, max-affine regression).

> What happens if we consider fitting with convex sets that are expressible via semidefinite programming?
  
1. Fitting Tractable Convex Sets to Support Function Evaluations, Y. S. Soh and [V. Chandrasekaran](http://users.cms.caltech.edu/~venkatc/), *Discrete and Computational Geometry*, Jan '21, <a href = "https://link.springer.com/article/10.1007/s00454-020-00258-0">[Article]</a> <a href = "http://arxiv.org/abs/1903.04194">[arXiv]</a> <a href = "http://github.com/yssoh/cvxreg">[Code]</a>

1. Learning Semidefinite Regularizers, Y. S. Soh and [V. Chandrasekaran](http://users.cms.caltech.edu/~venkatc/), *Foundations of Computational Mathematics*, Mar '18, <a href = "http://link.springer.com/article/10.1007/s10208-018-9386-z">[Article]</a> <a href = "http://arxiv.org/abs/1701.01207">[arXiv]</a> <a href = "https://github.com/yssoh/SDP_DL">[Code]</a>

1. Fitting Convex Sets to Data: Algorithms and Applications, Aug '18, [PDF](http://thesis.library.caltech.edu/11208/1/YongSheng_Soh_2019.pdf)
  
  
### Matrix Factorizations with Infinite Atoms

<img src="/assets/images/2x2_atoms.png" alt="Full range of SOCP atoms" width="800"/> <img src="/assets/images/2x2_full.png" alt="Reconstruction with SOCP atoms" width="800"/>

Given a data matrix Y, the matrix factorization task seeks a factorization of the form Y = A X, where A and X satisfies certain structural properties depending on the context.  In the simplest example, we impose that A and X have small inner dimension, with no further restriction -- this is simply the Singular Value Decomposition (SVD).  If for instance, if one is interested in representing the data vectors in Y via a _sparse_ _basis_, then one would impose (the columns of) X be sparse  -- this is known as dictionary learning or sparse coding.   If instead one wishes to explain the data via _non-negative_ components, then one seeks a _non-negative_ _matrix_ factorization.

One thing in common among these classical methods is that we compute a data matrix with _finitely_ many atoms.  However, there are settings in which this modelling assumption is inadequate -- perhaps, depending on the data, it is beneficial to instead learn dictionaries that contain _infinitely_ many atoms.  The central question in these works are:

> How do we learn matrix factorizations with _infinitely_ many atoms?  What does it mean to have dictionaries that have infinitely many atoms?  

> When is it beneficial to model data using _infinitely_ large dictionaries?

1. Multiplicative Updates for Symmetric-cone Factorizations, Y. S. Soh and <a href ="https://sites.google.com/site/antoniosvarvitsiotis/">A. Varvitsiotis</a>, *Mathematical Programming Series A*, <a href = "https://link.springer.com/article/10.1007/s10107-023-02015-6">[Article]</a> <a href = "https://arxiv.org/abs/2108.00740">[arXiv]</a>

1. A Non-commutative Extension of Lee-Seung's Algorithm for Positive Semidefinite Factorizations, Y. S. Soh and <a href ="https://sites.google.com/site/antoniosvarvitsiotis/">A. Varvitsiotis</a>, *NeurIPS*, 2021 <a href = "https://arxiv.org/abs/2106.00293">[arXiv]</a> <a href = "https://github.com/yssoh/PSD_MM">[Code]</a>

1. Learning Semidefinite Regularizers, Y. S. Soh and [V. Chandrasekaran](http://users.cms.caltech.edu/~venkatc/), *Foundations of Computational Mathematics*, Mar '18, <a href = "http://link.springer.com/article/10.1007/s10208-018-9386-z">[Article]</a> <a href = "http://arxiv.org/abs/1701.01207">[arXiv]</a> <a href = "https://github.com/yssoh/SDP_DL">[Code]</a>

1. Dictionary Learning under Symmetries via Group Representations, <a href ="https://subhro-ghosh.github.io/">S. Ghosh</a>, A. Y. R. Low, Y. S. Soh, Z. Feng, B. K. Y. Tan, *pre-print*, Jun '23, <a href = "https://arxiv.org/abs/2305.19557">[arXiv]</a>

1. Group Invariant Dictionary Learning, Y. S. Soh, *Transactions on Signal Processing*, Jun '21, <a href = "https://ieeexplore.ieee.org/document/9461688">[Article]</a> <a href = "https://arxiv.org/abs/2007.07550">[arXiv]</a> <a href = "https://github.com/bkytan/gidl">[Code] (maintained by Brendan KY Tan)</a>



