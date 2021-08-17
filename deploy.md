1) Downloading TensorRT.
TensorRT 8.0.1 GA for Ubuntu 18.04 and CUDA 10.2 DEB local repo package
https://developer.nvidia.com/compute/machine-learning/tensorrt/secure/8.0.1/local_repos/nv-tensorrt-repo-ubuntu1804-cuda10.2-trt8.0.1.6-ga-20210626_1-1_amd64.deb

2)Install TensorRT from the Debian local repo package. Replace ubuntuxx04, cudax.x, trt8.x.x.x and yyyymmdd with your specific OS version, CUDA version, TensorRT version and package date.
```
os="ubuntuxx04"
tag="cudax.x-trt8.x.x.x-yyyymmdd"
sudo dpkg -i nv-tensorrt-repo-${os}-${tag}_1-1_amd64.deb
sudo apt-key add /var/nv-tensorrt-repo-${os}-${tag}/7fa2af80.pub

sudo apt-get update
sudo apt-get install tensorrt
```
```
sudo apt-get install python3-libnvinfer-dev
```
```
sudo apt-get install uff-converter-tf
```
```
sudo apt-get install onnx-graphsurgeon
```
```
dpkg -l | grep TensorRT
```
