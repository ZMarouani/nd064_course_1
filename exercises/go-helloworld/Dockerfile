FROM golang:1.14.3-alpine
WORKDIR /go/src/app
ADD . .

RUN go mod init
RUN go mod tidy
RUN go build -o helloworld
EXPOSE 6111
CMD ["./helloworld"]