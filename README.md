# freessl
1- Download CertBot for windows:
https://dl.eff.org/certbot-beta-installer-win32.exe

2- Open Command Prompt as Administrator. (You can search for CMD in start menu and right click on it then select Run as Administrator).

3- run these commands in CMD (substitute youremailaddress with your real email address and yourdomain.com with your domain)
```
cd C:\Program Files (x86)\Certbot
```
```
certbot certonly --manual --preferred-challenges=dns   --email youremailaddress@gmail.com --server https://acme-v02.api.letsencrypt.org/directory -d *.yourdomain.com -d yourdomain.com
```
At first run, you will be asked to accept the Terms of Service and you should write "Y" and hit Enter.

if you don't want to enter your email address you can simply change the command like this:
```
certbot certonly --manual --preferred-challenges=dns   --register-unsafely-without-email --server https://acme-v02.api.letsencrypt.org/directory -d *.yourdomain.com -d yourdomain.com
```
