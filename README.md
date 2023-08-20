# Notes of setting up Immich server and using nginx as a reverse proxy for subdomain on QNAP NAS (TS-453Be, QTS 5.0.1.2425)




## 1. Create a shared folder for immich
![image](https://github.com/ForisC/note_immich_qnap/assets/52095287/f84dbdda-aa4c-4165-94a0-603b3f978352)

## 2. ssh to NAS and cd to the folder

```
ssh YourAccound@YourIP -p YourPort
YourAccound@YourIP's password:
[~] #
[~] # cd /share/immich
[/share/immich] #
```


## 3. Download the required files
  Immich offers several installation methods, including:

* Install Script
* Docker Compose

Docker Compose is the officially recommended method.

https://documentation.immich.app/docs/install/docker-compose

Download docker-compose.yml and example.env, either by running the following commands:
```
wget https://github.com/immich-app/immich/releases/latest/download/docker-compose.yml
```
```
wget -O .env https://github.com/immich-app/immich/releases/latest/download/example.env
```


ref. 

https://www.alvinchen.club/2018/11/06/reverse-proxy-on-nginx-docker-%E4%BD%BF%E7%94%A8qnap-container-station/
