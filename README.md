# zap-on-webgoat
The web pentesting is perfomed on the webgoat using the ZAP . In this i described about some of the common attack and their prevention
# zap on kali linux

first of all you have to download webgoat . search webgoat on your browser and owasp webgoat 
<img width="414" height="470" alt="image" src="https://github.com/user-attachments/assets/54610f6e-dc84-4647-a3ce-f6d5a79b0455" />

go at standard jars and then github page will be open . then click on webgoat which is at top and then 

<img width="851" height="650" alt="image" src="https://github.com/user-attachments/assets/415b5e59-58df-4952-8fbe-1e6935eb2e3b" />

go for webgoat.jar and download this . as this will be in download so

sudo apt update 
sudp apt upgrade
cd Downloads
java -jar webgoat(press tab now)

then this will run if you dont find java compatible version then download this from oracle and download and install (also run "sudo dpkg -i jdk-25.0.1_linux-x64_bin.deb" by locating cd download and install)

then after running this you will see the link  at the bottom " http://127.0.0.1:8080/WebGoa" copy (after chosing press shift+ctrl+c)

now open ZAP by searching in linux
open and past the link ( there only one search bar where http were already written remove this and past the link ctrl+v ) and chose active scan wait a while then this will give you list where you can read about them )



# NMAP


now to use nmap you have to open new terminal while running webgoat . 
nmap 127.0.0.1 -sV (this will tell the version of running service on a port )
nmap 127.0.0.1 --script http-sql-injection (this will tell that sql can be perfomed or not )
nmap 127.0.0.1 --script http-xssed (this will tell about cross site script attack is possible )
Nmap 127.0.0.1 -p-   (This will scan all the top 1000 ports and tell which are open and which are closed )
you can search on youtube "how to perfome pentesting on site using webgoat" remmember use 127.0.0.1 if you are usign the localhost for pentesting otherwise also you can use the thing youtuber told to use (like vulnhub.com )
