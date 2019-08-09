# Installing-PyCrypto-manually-Ubuntu-18-python3.6
How to Install PyCrypto since its not longer supported or discontinued you cant download it or use pip install it will generate errors

Requirements:
-Virtualenv
-python3
-pycrypto-2.6.1.zip

run
```
sudo apt update

sudo apt-get install gcc python3 python-dev python3-dev \
     build-essential libssl-dev libffi-dev \
     libxml2-dev libxslt1-dev zlib1g-dev \
     python-pip
```

### Download it manually
https://pypi.org/project/pycrypto/#files
or
```
cd <your-virtualenv-dir>/

source bin/activate

sudo wget https://files.pythonhosted.org/packages/60/db/645aa9af249f059cc3a368b118de33889219e0362141e75d4eaf6f80f163/pycrypto-2.6.1.tar.gz

tar -zxvf pycrypto-2.6.1.tar.gz

#move the folder your site-packages
mv pycrypto-2.6.1 /lib/python3.6/site-packages/pycrypto-2.6.1

cd /lib/python3.6/site-packages/pycrypto-2.6.1/

python setup.py build

python setup.py install
```


