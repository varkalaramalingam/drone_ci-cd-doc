FROM python:alpine3.6

ENV AWSCLI_VERSION "1.18.124"

RUN apk add --no-cache jq bash curl git wget && \
pip install awscli==$AWSCLI_VERSION

RUN curl -LO https://storage.googleapis.com/kubernetes-release/release/v1.18.0/bin/linux/amd64/kubectl && chmod +x ./kubectl && mv ./kubectl /usr/local/bin/kubectl

#docker build -t ramalingam81/awscli-kubectl .
#docker push ramalingam81/awscli-kubectl
#https://github.com/honestbee/awscli
