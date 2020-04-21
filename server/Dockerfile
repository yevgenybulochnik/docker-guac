FROM ubuntu:latest as powerline
RUN apt-get update -y && apt-get install git -y
RUN git clone https://github.com/powerline/fonts.git /root/fonts
RUN /root/fonts/install.sh

FROM guacamole/guacd
RUN apt-get update -y && apt-get install \
    git ttf-ancient-fonts -y
COPY --from=powerline /root/.local/share/fonts /root/.local/share/fonts
