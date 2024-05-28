FROM golang:latest

WORKDIR /usr/src/app

COPY go*.*/ .

RUN go mod tidy

COPY . .

ENV REQUEST_ORIGIN=http://localhost:5000

RUN go build -o server .

EXPOSE 8080

ENV PORT=8080


CMD ["./server"]
