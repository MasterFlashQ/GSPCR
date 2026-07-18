# GSPCR


## *GSPCR:4-DoF Global Spatial Consistency Graph for Point Cloud Registration with Repetitive Local Features*


# About
*The complete code will be released after the paper is accepted.*

# About
<img width="9312" height="3653" alt="图片1" src="https://github.com/user-attachments/assets/a9487c23-e17e-49e6-bd32-7e4c610241e7" />


GSPCR can sovle 4-DOF registration problem between two 3D point clouds.It achieves highly robust registration in scenarios characterized by extremely scarce initial correspondences and abundant repetitive geometric structures.

# Getting started


## Envoriment:
Our program is lightweight and can be included in any project that adds the PCL and CGAL library. We've tested it on Windows (VS2022)
## Dependencies:
1. PCL
2. CGAL
## Parameter configuration:
1.GSPCR needs to get the correspondences and sampled point cloud before running, we use the strategy of (downsampling) + (key point extraction) + (FPFH descriptor) + (correspondences matching) to generate initial correspondences. And we use Farthest point sample to sample the origin point clouds.
2.There are only one parameters of GSPCR: downsampling resolution. Furthermore, the number of sampled points also influences the accuracy and efficiency of the algorithm, which is primarily determined by the employed downsampling algorithm.
