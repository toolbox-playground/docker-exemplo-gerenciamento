# Roteiro de Exercícios para Comandos Docker

## Parte 2: Comandos Intermediários

### 1. docker kill

Para um contêiner imediatamente

**Tarefa:**
- Execute um contêiner utilizando `docker run -d nginx`.
- Utilize o comando `docker ps` para identificar o ID do contêiner criado.
- Utilize `docker kill <CONTAINER ID>` para parar o contêiner imediatamente.
- Verifique o estado do contêiner com `docker ps -a` para confirmar que ele está parado.

### 2. docker rm
Remove um contêiner parado.

**Tarefa:**

- Remova o contêiner parado no exercício anterior usando `docker rm <CONTAINER ID>`.
- Verifique se o contêiner foi removido utilizando `docker ps -a`.

### 3. docker stats
Monitora as estatísticas de uso de CPU, memória e rede de um contêiner.

**Tarefa:**
- Execute um contêiner com o comando `docker run -d nginx`.
- Monitore as estatísticas do contêiner usando `docker stats <CONTAINER ID>`.

### 4. docker pull
Baixa uma imagem do Docker Hub.

**Tarefa:**
- Baixe a imagem `alpine` usando `docker pull alpine`.
- Verifique se a imagem foi baixada com sucesso usando `docker images`.
  
### 5. docker push
Faz o push de uma imagem para o Docker Hub.

**Tarefa:**
- Crie uma tag para a imagem `my-curl` criada anteriormente e suba a imagem para o seu repositório Docker Hub utilizando o comando `docker tag my-curl <seu-usuario-dockerhub>/my-curl`.

- Faça o push da imagem com tag para o Docker Hub usando `docker push <seu-usuario-dockerhub>/my-curl`.