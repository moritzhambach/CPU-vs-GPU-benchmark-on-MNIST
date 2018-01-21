# CPU-vs-GPU-benchmark-on-MNIST

System: i7 8550U (4 cores), 16 GB ram, Geforce MX150 (2GB), windows 10
        using CUDA toolkit 8.0.16, CuDNN 8.0, python 3.5, keras 2.1.2 with tensorflow 1.4.0, visual studio 2015. The CUDA installation is easiest done by following the instructions in [link](http://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html) .


Training of neural networks can be accelerated by using the parallelism of calculations on GPUs. But by how much, for a typical small convolutional neural network? Let's find out! Here I compare training duration of a CNN with CPU or GPU for different batch sizes (see ipython notebook in this repo). The GPU load is monitored in an independent program (GPU-Z). 

Here's the result:

![alt text](https://user-images.githubusercontent.com/33765868/34654656-19171952-f3ff-11e7-9d1b-2f7c1ff8333b.png)

We can see that the GPU calculations with Cuda/CuDNN run faster by a factor of 4-6 depending on the batch sizes (bigger is faster).
