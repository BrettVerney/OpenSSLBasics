# OpenSSLBasics

openssl-new -out csr.pem -newkey rsa:2048 -nodes -sha256 -keyout key.pem -config openssl.cnf

openssl req -text -noout -verify -in csr.pem
