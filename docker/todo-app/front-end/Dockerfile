# rode a partir da imagem do node na versão 14
FROM node:14 AS todofrontend

# diretorio de trabalho
WORKDIR /app

# exponha a porta 3001
EXPOSE 3000

# adicione o arquivo node_modules.tar.gz à imagem
ADD node_modules.tar.gz .

# copie todos os arquivos da pasta back-end para a imagem. 
# (você pode usar o caminho relativo, lembrando que a Dockerfile está em ./docker/todo-app/back-end/Dockerfile);
COPY . .

# inicie a aplicação com o comando npm start respeitando as seguintes restrições
ENTRYPOINT ["npm"]
CMD ["start"]
