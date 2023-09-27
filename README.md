# wott-client
The project replicates a digital twin of a large-scale vision-based tactile sensor based on a WoTT framework. 

## Preliminary connection test
Install namp tool
```
sudo apt-get update
```
```
sudo apt-get install nmap
```
Then, scan active ports on our server PC.
```
nmap -p- -sV 150.65.152.71
```
You should see that 9090/tcp, 9292/tcp, and 9393/tcp ports are discovered and opened.

## About The wott-client

 - This project implements:

A WoT client that consumes the tactile information exposed by WoTT server running at JAIST over the Internet network.
   
## Dependencies
- wotpy
- numpy
- matplotlib

## Getting Started
The Wott client code should be run on a Ubuntu-OS computer.
Please make sure to add the domain name of the server machine to your local computer (Ubuntu):
```
$ sudo nano /etc/hosts
```
Then add:
```
$ 150.65.152.71  	ho-lab
```
[150.65.xxx.xx] is the ip address of JAIST WoTT server.
Then run:
```
$ cd codes/
```
```
python WoTTClient.py
```

## Paper
[[PDF] Web of Tactile Things: Towards an Open and Standardized Platform for Tactile Things via the W3C Web of Things](https://github.com/Ho-lab-jaist/wott-client/blob/main/paper/CAiSE2022_WOTT.pdf)
### Citation
```
@InProceedings{10.1007/978-3-031-07481-3_11,
author="Pham, Van Cu
and Luu, Quan Khanh
and Nguyen, Tuan Tai
and Nguyen, Nhan Huu
and Tan, Yasuo
and Ho, Van Anh",
title="Web of Tactile Things: Towards an Open and Standardized Platform for Tactile Things via the W3C Web of Things",
booktitle="Intelligent Information Systems",
year="2022",
publisher="Springer International Publishing",
address="Cham",
pages="92--99",
}
```
