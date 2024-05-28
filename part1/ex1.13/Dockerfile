FROM golang:latest

WORKDIR /usr/src/app

COPY go*.*/ .

RUN go mod tidy

COPY . .

RUN go build -o server .

EXPOSE 8080

ENV PORT=8080

CMD ["./server"]
