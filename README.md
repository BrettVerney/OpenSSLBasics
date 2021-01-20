# OpenSSLBasics
Instructions and examples for commonly used OpenSSL functions.

**Author:** Brett Verney</br>
**Version:** v0.1 | 20-01-2021

## Requirements

- OpenSSL software
- Organisation details
- Server details

## Instructions

1.) Open the file **openssl.cnf** with a text editor.
2.) Replace the example values with real information and save
3.) Using a CLI terminal run the command:

```openssl req -new -out server.csr -newkey rsa:2048 -nodes -sha256 -keyout private.key -config openssl.cnf```
