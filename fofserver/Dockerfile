# Prelude
FROM ubuntu
MAINTAINER Dillon "Ignotis" Morse

# Build
RUN apt-get update
RUN apt-get install lib32gcc1
RUN mkdir ~/steamcmd
RUN cd ~/steamcmd
RUN wget https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz
RUN tar -xvzf steamcmd_linux.tar.gz
RUN rm steamcmd_linux.tar.gz
RUN ./steamcmd +login anonymous +force_install_dir ~/fofserver +app_update 295230 +quit
# RUN echo "~/fofserver/$SERVER" > ~/.bashrc

# Run
EXPOSE 27015
