# OpenSSLBasics

openssl req -new -nodes -keyout key.pem -out csr.pem -config openssl.cnf

openssl req -text -noout -verify -in csr.pem
