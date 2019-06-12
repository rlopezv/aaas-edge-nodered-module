
AMD64

docker build --tag=edge-nodered-amd64 --file=latest/Dockerfile .

docker run -it -p 1880:1880 edge-nodered-amd64

docker tag edge-nodered-amd64 rlopezviana/aaas-edge-nodered:0.0.2-amd64

docker push rlopezviana/aaas-edge-nodered:0.0.2-amd64


For rPI it's required to execute in a rPi.
docker build --tag=edge-nodered-rpi --file=rpi/Dockerfile .

docker run -it -p 1880:1880 edge-nodered-rpi

docker tag edge-nodered-rpi rlopezviana/aaas-edge-nodered:0.0.2-arm32v7

docker push rlopezviana/aaas-edge-nodered:0.0.2-arm32v7

