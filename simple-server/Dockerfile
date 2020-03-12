FROM golang:latest
RUN mkdir /app
WORKDIR /app
COPY go.mod ./
RUN go mod download
ADD . /app/
RUN go build -o main .
EXPOSE 8080
CMD ["./main"]
