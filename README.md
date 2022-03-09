# VNC_setting
from windows10 remote to ubuntu 20.04

## 1.Set Vnc server on ubuntu

### Update package
* sudo apt update -y
* sudo apt upgrade -y
* sudo apt install tasksel -y

### Just choose "ubuntu desktop", others that are selected can be ignored
* sudo tasksel


### If using desktop version, you can skip this command
* systemctl set-default graphical.target


### Download vnc server
* sudo apt install tigervnc-standalone-server -y

### Choose an user, or add one
* adduser uservnc 
* su - uservnc

### After choosing user, create a vnc password
*  vncpasswd

![image](https://github.com/u11334342/VNC_setting/blob/main/result1.PNG)

### Enable Vnc server
*  vncserver -localhost no

![image](https://github.com/u11334342/VNC_setting/blob/main/result2.PNG)

### If succeed, it will be like below

![image](https://github.com/u11334342/VNC_setting/blob/main/result3.PNG)




