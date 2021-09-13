# De onde deve ser pega a imagem e a versão. Nesse caso do repositório padrão do Docker, a imagem do node

# FROM node:alpine
FROM daveamit/node-alpine-grpc:v9.0.0

# Autor/Mantenedor
# MAINTAINER Jonathan Baraldi

# Prover camada de cached para os módulos do Node
WORKDIR /tmp
RUN npm install

RUN mkdir -p /src 
	# Instalar MariaDB SQL e rodar o script para injetar o SQL

RUN npm install mysql@2.18.1
	# Definir diretório de trabalho
WORKDIR /src
COPY . /src

	# Expor porta 80
EXPOSE  8080

	# Rodar o app usando nodemon
CMD ["node", "/src/index.js"]