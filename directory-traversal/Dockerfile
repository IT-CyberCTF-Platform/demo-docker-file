FROM ubuntu:22.04
ENV TZ=Asia/Bangkok
ENV DEBIAN_FRONTEND=noninteractive
RUN apt update
RUN apt-get install -y git php
RUN git clone https://github.com/IT-CyberCTF-Platform/demo-vulnerabe-app.git
RUN mv demo-vulnerabe-app/directory-traversal/php/ lab/
RUN rm -fr demo-vulnerabe-app/
WORKDIR /lab
EXPOSE 80
CMD ["php", "-S","0.0.0.0:80"] 
