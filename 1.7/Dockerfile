FROM ubuntu:16.04

RUN apt-get update && apt-get install -y curl wget

CMD echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website