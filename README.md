# Colab-TF20-TF-TRT-inference-from-Keras-saved-model

# 代码运行成功时的环境
* Ubuntu 18.04
* cuda 10.1
* TensorRT 6.0.1
* Tensorflow 2.1

> 注意：此环境的选择是根据彼此之间的官方的环境要求，筛选后的搭配。搭配的此时，官方给出的经过测试的构建配置，最高为
> [tensorflow 2.1 cuda 10.1](https://www.tensorflow.org/install/source?hl=zh-cn#gpu) 。
> 根据cuda版本，选择[TensorRT版本](https://developer.nvidia.com/zh-cn/tensorrt)  。
> 由于支持cuda 10.1 的TensorRT最高版本为为6.0.15，因此安装的该版本

# 环境配置
## 1、cuda 10.1的配置 
官方安装教程在此：[链接](https://developer.nvidia.com/cuda-10.1-download-archive-base?target_os=Linux&target_arch=x86_64&target_distro=Ubuntu&target_version=1804&target_type=deblocal) \
安装完后有个官方的教程测试是否正确安装：[CUDA Quick Start Guide](https://docs.nvidia.com/cuda/cuda-quick-start-guide/index.html#redhat-x86_64-rpm)

## 2、TensorRT 6.0.1的配置
官方安装教程在此：[链接](https://docs.nvidia.com/deeplearning/tensorrt/install-guide/index.html#installing-debian) \
教程中有测试是否正确安装

## 3、Tendorflow的配置
* 安装`miniconda`，如果本地没有
* 在存放`environment.yml`的路径下执行：`conda env create -f environment.yml`

# 执行
在`tf_2.1`的环境中执行`jupyter notebook`，打开工程中的`.ipynb`文件
> `.ipynb`文件中并非所有的都需要执行，具备一定基础的可以明白里面的内容 \
> `data/` 文件夹中保存的是该工程中会下载的四张图片，如果网络不好可以注释掉下载的代码，直接使用这四张图片