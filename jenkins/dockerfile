FROM ubuntu:18.04
RUN  apt-get update
RUN  apt-get install -y apache2 curl net-tools wget unzip
RUN  wget https://www.free-css.com/assets/files/free-css-templates/download/page296/carvilla.zip ;
RUN  mkdir -p /var/www/html/
RUN  unzip carvilla.zip
RUN  cp -r carvilla-v1.0/* /var/www/html/
ENTRYPOINT apachectl -D FOREGROUND
