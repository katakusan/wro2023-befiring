# Yolov5 downlode 

## To download the required dependencies

```
sudo apt update
sudo apt install -y python3-pip
pip3 install --upgrade pip
```
downlode pip

```
git clone https://github.com/ultralytics/yolov5
cd yolov5
gedit requirements.txt
```

at this moment you will into the requirements.txt
we need to modfication some  version of the suite

```
gitpython>=3.1.20
matplotlib==3.2.2
numpy==1.19.4
```
modfication gitpython matplotlib and  numpy version

```
# torch>=1.7.0
# torchvision>=0.8.1
# ultralytics
```
mark torch torchvision ultralytics don't let to download

```
sudo apt install -y libfreetype6-dev
```

install this package to help install requirements.txt

```
pip3 install -r requirements.txt
```
Start installing the requirements.txt dependencies (please be patient as it may take some time)

Don't worry if you encounter any error messages, they will be addressed later.

## Download Pytorch

** we download pytorch version is 1.10 **

```
cd

wget https://nvidia.box.com/shared/static/fjtbno0vpo676a25cgvuqc1wty0fkkg6.whl -O torch-1.10.0-cp36-cp36m-linux_aarch64.whl

pip3 install torch-1.10.0-cp36-cp36m-linux_aarch64.whl
```
wait some time and pytorch will be download

## Download Torchvision

```
cd
sudo apt install -y libjpeg-dev zlib1g-dev
git clone --branch v0.9.0 https://github.com/pytorch/vision torchvision
cd torchvision
sudo python3 setup.py install
```

wait some time and Torchvision will be download

Next open yolov5 folder to test and check for any missing dependencies

**If you missing any dependencies print this code**

```
pip3 install {you miss dependencies}
```
If you missing dependencies is ultralytics you need to download python 3.8 to download it

[python 3.8 download teach](https://github.com/katakusan/wro2023-/blob/main/Jetson%20nano/yolov5/python3.8.md)


[**_back to README.md_**](https://github.com/katakusan/wro2023-befiring/blob/main/README.md)


