FROM golang:latest AS build

WORKDIR /app

COPY . ./
RUN go mod download

RUN go build -o /bin/app

EXPOSE 1323

CMD [ "/bin/app" ]