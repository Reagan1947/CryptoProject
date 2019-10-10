# CryptoProject 多云服务器加密项目
This project based on paper 《Provably Secure Fine-Grained Data Access Control over Multiple Cloud Servers in Mobile Cloud Computing 
Based Healthcare Applications》

这是一个基于论文《Provably Secure Fine-Grained Data Access Control over Multiple Cloud Servers in Mobile Cloud Computing Based Healthcare 
Applications》实现的多云服务器加密项目

# Enviroment环境
* Ubuntu 18LTS
* Python3.6
* Charm-crypto


# How to install Charm-crypto on Ubuntu18LTS <br> 如何在Ubuntu18LTS中安装Charm-crypto
```
sudo apt-get install subversion 
sudo apt-get install m4 
sudo apt-get install flex 
sudo apt-get install bison 
sudo apt-get install libssl-dev 
sudo apt-get install python3-setuptools python3-dev 
sudo apt-get install libgmp-dev 
wget http://crypto.stanford.edu/pbc/files/pbc-0.5.14.tar.gz 
tar xf pbc-0.5.14.tar.gz 
cd pbc-0.5.14 
./configure && make && sudo make install 
```

Dowload Charm-crypto from [https://pypi.python.org/pypi/charm-crypto/0.43](https://pypi.python.org/pypi/charm-crypto/0.43):<br>
从 [https://pypi.python.org/pypi/charm-crypto/0.43](https://pypi.python.org/pypi/charm-crypto/0.43)
下载魅力的tar.gz文件，提取，改变目录，那么：

```
./configure.sh 
sudo make 
sudo make install 
sudo ldconfig 
```
Charm-crypto have to use Openssl 1.X.X so you need to install Openssl 1.0.2. Even Ubuntu 18LTS have installed Openssl 1.1.1 or other.:<br>
因为在Ubuntu18.04.3中Openssl版本高于Charm-crypto要求版本，降低Openssl版本：
```
wget https://www.openssl.org/source/openssl-1.0.2l.tar.gz
tar -xzvf openssl-1.0.2l.tar.gz
cd openssl-1.0.2l
./config --prefix=/usr/local --openssldir=/usr/local/openssl 
sudo make
sudo make install
```
# To do list 任务清单
- [x]  解决dict在数据库中的存储问题。
- [ ]  Django多数据库实现问题
- [ ]  应用于Django项目上
- [ ]  GUI界面
