# OpenSSLBasics
Instructions and examples for commonly used OpenSSL functions.

**Author:** Brett Verney</br>
**Version:** v0.2 | 28-09-2022

## Requirements

- OpenSSL software
- Organisation details
- Server FQDN details

## Instructions

1.) Open the file **openssl.cnf** with a text editor</br>
2.) Replace the example values with real information and save (see req_ext_examples.txt) </br>
3.) Using a CLI terminal run the command:</br></br>
```openssl req -new -out server.csr -newkey rsa:2048 -nodes -sha256 -keyout private.key -config openssl.cnf```</br></br>
4.) Verify the contents of the CSR with the following command:</br></br>
```openssl req -in server.csr -noout -text```</br></br>
5.) Save private key in a password safe application</br>
6.) Submit CSR to CA to sign</br>
7.) Import CA signed certificate, any root and/or imtermediate certificates, and private key to servers</br>
8.) Optionally combine the signed certificate with the private key to PKCS12 format with the following command:</br></br>
```openssl pkcs12 -export -out server.p12 -in server.cer -inkey private.key -passin pass:secure_password -passout pass:secure_password```</br></br>
