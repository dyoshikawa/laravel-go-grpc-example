FROM golang:1-alpine
MAINTAINER dyoshikawa

RUN apk update
RUN apk add git bash
RUN go get -u -v github.com/golang/dep/cmd/dep

COPY . /go/src/bitbucket.org/crunchtimer/pwcp/helloworld_client
WORKDIR /go/src/bitbucket.org/crunchtimer/pwcp/helloworld_client

CMD go run main.go