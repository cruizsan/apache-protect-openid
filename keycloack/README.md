# Protect Apache route with Keycloack

## Configuration apache
See admin.conf

## Configuration Keycloack
- Create new Realm (admin.me)
![alt](https://github.com/cruizsan/apache-protect-openid/raw/master/keycloack/img/001.PNG)
- Create new Client (admin.me)
  - Client ID : admin.me
  - Enabled : ON
  - Client Protocol : openid-connect
  - Access Type : confidential
  - Standard Flow Enabled : ON
  - Direct Access Grants Enabled : ON
  - Valid Redirect URIs : https://admin.me/*
  - Base URL = https://admin.me
![alt](https://github.com/cruizsan/apache-protect-openid/raw/master/keycloack/img/002.PNG)
![alt](https://github.com/cruizsan/apache-protect-openid/raw/master/keycloack/img/003.PNG)
- Create secret
![alt](https://github.com/cruizsan/apache-protect-openid/raw/master/keycloack/img/004.PNG)
