# CPU-vs-GPU-benchmark-on-MNIST

System: i7 8550U (4 cores), 16 GB ram, Geforce MX150 (2GB), windows 10
        using Cuda toolkit 8.0.16, CuDNN 8.0, python 3.5, keras 2.1.2 with tensorflow 1.4.0, visual studio 2015

Training of neural networks can be accelerated by using the parallelism of calculations on GPUs. But by how much, for a typical small convolutional neural network? Let's find out! Here I compare training duration of a CNN with CPU or GPU for different batch sizes. The GPU load is monitored in an independent program (GPU-Z). 

Here's the result:

![link](![alt text](https://user-images.githubusercontent.com/33765868/34654402-5dc7eddc-f3fb-11e7-9148-0ac42a453c5a.png)
