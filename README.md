# https-localhost-ssl-certificate
Create a local trusted certificate for a local HTTPS server (https://localhost)

## Overview
This script can create local generated SSL certificates to be used in a local web server environment (For example: Node.js/Express)

## Requirements

* `openssl` library to generate certificates and keys
* A local HTTPS-enabled web server to test your certificate

## Certificate Instalation

* Modify the file `server.csr.cnf` to match your country, state company, organization details 
  * `C=[2-letter Country Code]`
  * `ST=[State/Province]`
  * `L=[Location/City]`
  * `O=[Organization/Company]`
  * `OU=[Organizational Unit]`
  * `emailAddress=[admin@email]`
  * `CN=localhost` (You may keep this value unless you are securing a different local host name)
* Execute the script `sslcert.sh`, to generate `server.crt` and `server.key`
* Put thsese files accesible to configure your web server 
  * `server.key` as the private key
  * `server.crt` as the server certificate


## References

https://medium.freecodecamp.org/how-to-get-https-working-on-your-local-development-environment-in-5-minutes-7af615770eec



