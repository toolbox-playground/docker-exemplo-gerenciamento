# Roteiro de Exercícios para Comandos Docker

## Parte 3: Comandos Avançados

### 1. docker images
Lista todas as imagens no sistema.

**Tarefa:**
- Execute o comando `docker images`.
- Observe as colunas mostradas e entenda o que cada uma representa.

### 2. docker start
Inicia um contêiner previamente parado.

**Tarefa:**
- Inicie um contêiner previamente parado usando `docker start <CONTAINER ID>`.

### 3. docker restart
Reinicia um contêiner em execução.

**Tarefa:**
- Reinicie um contêiner em execução usando `docker restart <CONTAINER ID>`.

### 4. docker rmi
Remove uma imagem do sistema.

**Tarefa:**
- Remova uma imagem usando `docker rmi <CONTAINER ID ou NAME da imagem>`.
- Verifique se a imagem foi removida usando `docker images`.

### 5. docker exec
Executa um comando dentro de um contêiner em execução.

**Tarefa:**
- Execute um comando dentro de um contêiner em execução usando `docker exec -it <CONTAINER ID> bash`.
- Explore o shell do contêiner e execute comandos como `ls`, `ps`, etc.

### 6. docker logs
Verifica os logs de um contêiner em execução.

**Tarefa:**
- Verifique os logs de um contêiner em execução usando `docker logs <CONTAINER ID>`.

### 7. docker inspect
Investiga detalhes de um contêiner, imagem ou rede.

**Tarefa:**
- Use o comando `docker inspect <CONTAINER ID ou imagem>` e observe os detalher do contêiner ou da imagem.

### 8. docker cp
Copia arquivos ou diretórios entre o sistema host e um contêiner.

**Tarefa:**
- Execute o contêiner usando `docker run -d --name meu_nginx nginx`.
- Use o comando `docker cp index.html nginx:/usr/share/nginx/html/index.html` para copiar o arquivo `index.html` do sistema host para dentro do contêiner `meu_nginx`, no diretório `/usr/share/nginx/html/`.
- Verifique se o arquivo foi copiado corretamento utilizando o comando `docker exec -it meu_nginx ls /usr/share/nginx/html/`.

### 9. docker system prune
Limpa recursos não utilizados, como contêineres parados e imagens não utilizadas.

**Tarefa:**
- Limpe recursos não utilizados usando `docker system prune`.

### 10. docker save/load
Salva e carrega imagens Docker.

**Tarefa:**

- Salve uma imagem Docker em um arquivo tar usando `docker save -o <nome_do_arquivo>.tar <nome_da_imagem>`.

- Carregue uma imagem Docker a partir de um arquivo tar usando `docker load -i <nome_do_arquivo>.tar`.
