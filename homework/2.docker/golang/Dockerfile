FROM golang:1.19.0
WORKDIR /app
RUN apt update
RUN go version
EXPOSE "8080"
COPY go.* ./
RUN go mod download
COPY . .
RUN go build -o main-service ./main.go
CMD ["./main-service"]