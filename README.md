###start Django example commands
user@S0736:~/Desktop/mysite$ docker build -t Django .

user@S0736:~/Desktop/mysite$ docker run -d -p 8000:8000 Django


###start Nginx example commands
user@S0736:~/Desktop/mysite/nginx$ docker build -t nginx .

user@S0736:~/Desktop/mysite/nginx$ docker run -d -p 80:80 nginx


