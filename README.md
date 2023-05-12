# wott-client
The project replicates a digital twin of a large-scale vision-based tactile sensor based on a WoTT framework. 

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
$ 150.65.152.91  	ho-lab
```
[150.65.xxx.xx] is the ip address of JAIST WoTT server.
Then run:
```
$ cd codes/
```
```
python WoTTClient.py http://150.65.152.91:9090/tactilesensor-5fd1037e-1c8c-df9e-7136-ebfb938fc625
```
where ```http://150.65.152.91:9090/tactilesensor-5fd1037e-1c8c-df9e-7136-ebfb938fc625``` is the url for WoTT application that exposes property affordances of TacLink device. Please modify according to your needs.
