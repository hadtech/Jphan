FROM bitnami/moodle:latest
RUN mv /opt/bitnami/apache2/conf/bitnami/certs/server.crt /opt/bitnami/apache2/conf/bitnami/certs/server.crt.backup
RUN mv /opt/bitnami/apache2/conf/bitnami/certs/server.key /opt/bitnami/apache2/conf/bitnami/certs/server.key.backup
COPY server.key /opt/bitnami/apache2/conf/bitnami/certs/server.key
COPY server.crt /opt/bitnami/apache2/conf/bitnami/certs/server.crt
RUN mv /opt/bitnami/apache2/conf/httpd.conf /opt/bitnami/apache2/conf/httpd.conf.backup
COPY httpd.conf /opt/bitnami/apache2/conf/httpd.conf

