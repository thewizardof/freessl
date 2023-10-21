# freessl
1- Download CertBot for windows:
https://dl.eff.org/certbot-beta-installer-win32.exe

2- Open Command Prompt as Administrator. (You can search for CMD in start menu and right click on it then select Run as Administrator).

3- run these commands in CMD (substitute youremailaddress with your real email address and yourdomain.com with your domain)
```
cd C:\Program Files (x86)\Certbot
```
```
certbot certonly --manual --preferred-challenges=dns   --email youremailaddress --server https://acme-v02.api.letsencrypt.org/directory -d *.yourdomain.com -d yourdomain.com
```

