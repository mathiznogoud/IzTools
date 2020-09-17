FROM alpine

RUN apk add nmap nmap-scripts masscan python3 py3-pip bash libxslt git sudo libpcap-dev
RUN mkdir /home/iznogoud
RUN cd /home/iznogoud && git clone https://github.com/mathiznogoud/massmap4docker
WORKDIR /home/iznogoud
CMD ["/bin/bash"]


#docker build -t massmapimg .
#docker run -it -d --name massmap --mount source=massmap,target=/home/iznogoud massmapimg
