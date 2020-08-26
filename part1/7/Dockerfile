FROM ubuntu:16.04
RUN apt-get update && apt-get install -y curl
COPY curlerScript.sh .
RUN chmod +x curlerScript.sh
CMD ./curlerScript.sh
