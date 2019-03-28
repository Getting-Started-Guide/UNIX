### Guide

1. determine whether openssl is already installed   
    `which openssl`   
    if `bash` shows `usr/bin/openssl` follow with step two, if not:   
    a) `sudo apt-get install openssl`   
    b) `sudo apt-get update`   
    c) `sudo apt-get upgrade`   

2. generate private key with a key length of 2048   
    `openssl genrsa -out *.<host>.<tld>.key 2048`

3. create csr file (Certificate Signing Request) and follow the instructions   
    `openssl req -new -key *.<host>.<tld>.key -out *.<host>.<tld>.csr`

#### create selfsigned certificate

1. create selfsigned certificate with with one year validity   
    `openssl x509 -req -days 365 -in *.<host>.<tld>.csr -signkey *.<host>.<tld>.key -out *.<host>.<tld>_selfsigned.crt`

2. determine the current path of the directory   
    `pwd`
