See http://code.google.com/p/iphone-dataprotection/wiki/README

#Usage

It works using OSX and the following:

- Xcode 4.3 (xcode_43_lion.dmg) => Can be download from https://developer.apple.com/downloads/
- SDK 5.0
- iTunes 11.1.1
- redsnow 0.9.15b3 (redsnow_mac_0.9.15b3) 


#Compilation instructions

In order to compile ramdisk tools, you need to follow the next steps:
- Copy "IOKit.frameworkHeaders" content to /Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS5.0.sdk/System/Library/Frameworks/IOKit.framework/Headers/."

# Installation 

## Santoku Linux 

- Install swig 

`
sudo apt-get install swig
`

- Install PIP

`
sudo apt-get install python-pip
` 

- Install Python dependencies

`
sudo pip install progressbar

sudo pip install setuptools

sudo pip install construct

sudo pip install pyasn1
`

## OSX

- Install swig

`
brew install swig
`

- Install M2Crypto

`
git clone https://github.com/M2Crypto/

python setup.py build build_ext --openssl=/usr/local/Cellar/openssl/1.0.2/

sudo python setup.py install build_ext --openssl=/usr/local/Cellar/openssl/1.0.2
`

- Install python modules

`
pip install progressbar 

pip install setuptools

pip install construct

pip install pyasn1

pip install M2Crypto-0.21.1-py2.7-macosx-10.9-intel.egg
`
- Install M2Crypto for OSX

`
curl -O http://chandlerproject.org/pub/Projects/MeTooCrypto/M2Crypto-0.21.1-py2.7-macosx-10.9-intel.egg

sudo easy_install M2Crypto-0.21.1-py2.7-macosx-10.9-intel.egg
`

- Install pycrypto

`
sudo ARCHFLAGS='-arch i386 -arch x86_64' easy_install pycrypto
