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

### Check Vnc server status
*  vncserver -list

![image](https://github.com/u11334342/VNC_setting/blob/main/result3.PNG)

### Shot down server by display id (my id is 2)
*  vncserver -kill :2

![image](https://github.com/u11334342/VNC_setting/blob/main/result4.PNG)

## Set Vnc viewer on windows10

### Go to file->new connection, enter your ip, port number and Name

![image](https://github.com/u11334342/VNC_setting/blob/main/result5.PNG)


