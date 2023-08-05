Open Jetson nano terminal 

```
sudo apt update
```

```
git clone https://github.com/ultralytics/yolov5
```
clone yolov5 file on your Jetson nano

download pytorch and torchvision

```
wget https://nvidia.box.com/shared/static/fjtbno0vpo676a25cgvuqc1wty0fkkg6.whl -O torch-1.10.0-cp36-cp36m-linux_aarch64.whl

pip3 install torch-1.10.0-cp36-cp36m-linux_aarch64.whl
```
wait some time and pytorch will be download

```
cd
sudo apt install -y libjpeg-dev zlib1g-dev
git clone --branch v0.9.0 https://github.com/pytorch/vision torchvision
cd torchvision
sudo python3 setup.py install
```

wait some time and Torchvision will be download

```
sudo apt upgrade
```

Upgrade 

```
sudo apt install build-essential libssl-dev zlib1g-dev libncurses5-dev libncursesw5-dev libreadline-dev libsqlite3-dev libgdbm-dev libdb5.3-dev libbz2-dev libexpat1-dev liblzma-dev libffi-dev libc6-dev
```

Install necessary packages.

```
wget https://www.python.org/ftp/python/3.8.12/Python-3.8.12.tar.xz
tar -xf Python-3.8.12.tar.xz
cd Python-3.8.12
./configure --enable-optimizations
make -j4 
sudo make altinstall
``` 
Install python3.8

```
python3.8 -m pip install --upgrade pip

python3.8 -m pip install yolov5
```

Update pip and download yolov5.

```
python3.8 detect.py --weights yolov5n6.pt --nosave --source 0
```

open yolov5 detect  (_weights version can be chang ex:yolov5s yolov5m......_)

**Beware: The number after "source" represents the camera name. The default name is usually 0. If there are more than two cameras set up, you can use the following code to find the camera.**

