PHONY: all

all:
	openssl genrsa -out any.key 1024
	openssl req -new -key any.key -out any.pem -sha1
	openssl x509 -in any.pem -out any.crt -req -signkey any.key -days 365 -sha1
	rm any.pem
