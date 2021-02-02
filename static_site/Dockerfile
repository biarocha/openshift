# Base image
FROM golang:latest

LABEL maintainer="Bia"

# Criando pasta /app na base image
RUN mkdir /app

# Copiando os arquivos da aplicacao para a pasta /app
ADD . /app

# Setando a pasta /app como Workdir
WORKDIR /app

# Executando o build da app
RUN go build -o main .

# Expondo a porta da app
EXPOSE 8080

# Comando de start da app
CMD ["./main"]