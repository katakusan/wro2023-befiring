
```
sudo apt upgrade
```

Upgrade your hardware environment.

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
cd

python3.8 -m venv myenv

source myenv/bin/activate

pip3 install ultralytics
```
Create an environment and install Ultralytics

[**_back to README.md_**](https://github.com/katakusan/wro2023-befiring/blob/main/README.md)


