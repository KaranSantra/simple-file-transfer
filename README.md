# simple-file-transfer

# Installation Guide
## Linux

Check if python3.8 is installed
```
python --version
sudo apt install python3.8
```
Check if pip3 is install
```
pip3 --version 
sudo apt install python3-pip
```
Install tqdm package
```
sudo /usr/bin/python3.8 -m pip3 install tqdm
(or)
pip3 install tqdm
```

## Windows 
** pray to Lord for forgiveness (send a pr)**

## Mac OS

** figure it out (send a pr)**
<br>
<br>

# User Guide
<big>For instance, if you want to send data.csv to Mitul (SERVER_HOST="192.168.x.xxx") listening @ SERVER_PORT=81</big>

I will ask Mitul to run reciever.py file with
SERVER_HOST = "192.168.x.xxx"
SERVER_PORT = 81

```
python3 reciever.py
```

Then I will run the following command from my pc
Syntax: 
```
python3 sender.py <file-path> <SERVER_HOST> --port=81
```
Example
```
python3 sender.py ./data.csv 192.168.1.123 --port=81
```

Mitul will terminate the server-instance, once the file is recieved

<b>Note:</b>
- filepath can be relative or absolute
- to send multiple file zip it then send
- if port number is not mentioned then default port is 5001



---------------------------------------
## CLI help
C:\> python sender.py --help
usage: sender.py [-h] [-p PORT] file host
```
Simple File Sender

positional arguments:
file                  File name to send
host                  The host/IP address of the receiver

optional arguments:
-h, --help            show this help message and exit
-p PORT, --port PORT  Port to use, default is 5001
```



Source:
https://github.com/x4nth055/pythoncode-tutorials/tree/master/general/transfer-files
