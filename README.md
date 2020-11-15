# nginx-print-headers

Simple container application to print headers. request body and Method of incoming http requests. It uses Openresty base container and print the requests using echo modules
https://www.nginx.com/resources/wiki/modules/echo/

# How to run ?

git clone git@github.com:betterltn/nginx-print-headers.git </br>
cd nginx-print-headers </br>
docker build . -t nginx-print-headers </br>
docker run -p 8000:8000 nginx-print-headers </br>


Use curl to access this application </br>

curl http://localhost:8000/ -H "test: hi"
GET / HTTP/1.1
Host: localhost:8000
User-Agent: curl/7.54.0
Accept: */*
test: hi
 

