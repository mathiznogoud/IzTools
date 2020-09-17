Build docker file
#docker build -t massmapimg .


Run the shit
#docker run -it -d --name massmap --mount source=massmap,target=/home/iznogoud massmapimg
