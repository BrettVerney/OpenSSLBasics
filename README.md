# OpenSSLBasics
Instructions and examples for commonly used OpenSSL functions.

**Author:** Brett Verney</br>
**Version:** v0.1 | 20-01-2021

## Requirements

- OpenSSL software
- Organisation details
- Server details

## Instructions

1.) Open the file **openssl.cnf** with a text editor</br>
2.) Replace the example values with real information and save</br>
3.) Using a CLI terminal run the command:</br>

```openssl req -new -out server.csr -newkey rsa:2048 -nodes -sha256 -keyout private.key -config openssl.cnf```</br>
4.) Verify the contents of the CSR with the following command:</br>
```openssl req -in mycsr.csr -noout -text```</br>
5.) Submit CSR to CA to sign</br>
6.) Import CA signed certificate, any root and/or imtermediate certificates, and private key to servers</br>
