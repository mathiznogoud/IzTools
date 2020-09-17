FROM alpine

RUN apk add nmap nmap-scripts masscan python3 py3-pip bash libxslt git sudo libpcap-dev
RUN mkdir /home/iznogoud
RUN git clone https://github.com/mathiznogoud/IzTools /home/iznogoud/MassMap
RUN cd /home/iznogoud/MassMap && git filter-branch --prune-empty --subdirectory-filter MassMapTools/Massmap4docker/ HEAD
WORKDIR /home/iznogoud/MassMap
CMD ["/bin/bash"]


#docker build -t massmapimg .
#docker run -it -d --name massmap --mount source=massmap,target=/home/iznogoud massmapimg
