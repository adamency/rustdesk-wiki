# How much does the community version of RustDesk server cost? 
The community releases are free of charge if you wish to self host, no license is required. 
# Can I host my own RustDesk server? 
- Yes, you can host your own RustDesk server 
- There's a guide here: https://rustdesk.com/docs/en/self-host/ 
# Where can I download RustDesk Sever?
You can download RustDesk sever from: 
- https://github.com/rustdesk/rustdesk-server 
- https://rustdesk.com/server 
# The server is asking me for a license, where can I get one from? 
Please ensure you have downloaded the newest release of RustDesk server as licenses are no longer required for the community release. 
# What does the server do, why do I need it? 
- It is primarily used to help your RustDesk clients to find each other. 
- Once this is done, it helps you try and get a direct connection between them. 
- If this fails and your client and controlled devices cannot talk directly to each other, the relay part of side the server will be used to handle the connection. 
# I only use RustDesk for a few devices on my local network with no Internet connectivity... Can I still use RustDesk? 
Yes, you can! 

By default this is turned off for security, however if wish to allow this you can do so by doing steps below: 
- On the device you wish to control 
- Go into the Menu and select Enable direct IP...  
- On the client you are connecting from you can now input the Local IP address or host name the address box and click connect. 

# hbbs -c,  the configuration file format
Supper simple format just a=b on each line, a is the name of the option you see from the --help. e.g.
e.g.
```
port=123456
```

You can also put them in .env file under the same directory of hbbs/hbbr. hbbs/hbbr reads .env file no matter if you specify -c. 
![image](https://user-images.githubusercontent.com/71636191/173327939-4ed089cc-81bc-416a-a22e-6abc2791cfc4.png)

# Web client

https://rustdesk.com/docs/en/dev/build/web/

http://web.rustdesk.com/ no https for the time being

# Change id, addressbook/api/login and web console?

https://github.com/rustdesk/rustdesk-server/issues/22

https://github.com/rustdesk/rustdesk/discussions/570

https://github.com/rustdesk/rustdesk/issues/509 

# Hardware requirement for RustDesk server.
The hardware requirements are very low, the minimum configuration of the cloud server is enough, and the CPU and memory requirements are the minimum. Regarding the network size, if the TCP hole punching direct connection fails, the relay traffic will be consumed. The traffic of a relay connection is between 30k-3M/s (1920x1080 screen), depending on the resolution settings and screen update. If it is only for office work demand, the traffic is around 100K/s. 

