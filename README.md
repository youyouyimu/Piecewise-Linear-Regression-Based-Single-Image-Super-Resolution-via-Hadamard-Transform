Requirements:
The code is developed with Matlab (R2015a) and was tested under Windows 7 (64 bit). The library "Eigen" is requried to use the code, which is for the mex/cpp files.

Building the code:
There is only a single mex/cpp file included in this package that can be build with the MATLAB function "mex". The steps are:

mex -setup C++                                                                 
mex SR_scale_Hadamard.cpp ("scale" is the upscaling factor,e.g. mex SR_2_Hadamard.cpp )
We provide a pre-compiled file "SR_2_Hadamard.mexw64" for Windows 7 (64 bit).

Using the code:
The file "SR_demo.m" is the demo usage of the proposed algorithm.
The file "SR_demo_urban100.m" is used to evaluate our method on Urban100.

The modcrop function is from the source code of: C. Dong, C. C. Loy, K. He, and X. Tang. Learning a deep convolutional network for image super-resolution. In European Conference on Computer Vision, pages 184¨C199. Springer, 2014.

The training dataset used in our paper can be generated by file "create_train_data.m".

The learned mapping models as well as the decision tree for scaling factor 2 can be directly used for SR reconstruction.

If you have problems with the code, please contact me at sejingjingluo@mail.scut.edu.cn
