FROM        nginx
RUN         rm -rf /usr/share/nginx/html/*
WORKDIR     /usr/share/nginx/html/
ADD         https://studentapi-cit.s3-us-west-2.amazonaws.com/studentapp-frontend.tar.gz studentapp-frontend.tar.gz
RUN         tar -xf studentapp-frontend.tar.gz
COPY        nginx.conf /etc/nginx/nginx.conf.tmp
COPY        run.sh /
RUN         chmod +x /run.sh
CMD         /run.sh
