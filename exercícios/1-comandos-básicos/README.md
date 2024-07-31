# Roteiro de Exercícios para Comandos Docker

## Parte 1: Comandos Básicos

### 1. docker ps

Lista todos os contêineres que estão em execução.

**Tarefa:**
- Execute o comando `docker ps`.
- Identifique seguintes as colunas:
    - `CONTAINER ID`: Identificação única do contêiner.
    - `IMAGE`: Imagem usada para criar o contêiner.
    - `COMMAND`: Comando que está sendo executado no contêiner.
    - `CREATED`: Tempo desde a criação do contêiner.
    - `STATUS`: Estado atual do contêiner (e.g., Up, Exited).
    - `PORTS`: Portas do contêiner para o host.
    - `NAMES`: Nome do contêiner.

### 2. docker run
 Baixa e executa determinada imagem.

**Tarefa:**
- Execute o comando `docker run hello-world`.
- Observe a mensagem de saída:
    - A mensagem deve indicar que a imagem `hello-world` foi baixada com sucesso.

### 3. docker stop
Para um contêiner em execução.

**Tarefa:**
- Execute o seguinte contêiner usando `docker run -d nginx` para iniciar o servidor web nginx.
- Identifique o ID ou o NOME do contêiner usando `docker ps`.
- Pare o contêiner com `docker stop <CONTAINER ID ou NAME do contêiner>`.
- Verifique se o contêiner foi parado corretamente executando novamente o comando `docker ps`.

### 4. docker build
Constrói uma imagem Docker personalizada.

**Tarefa:**
- Crie um diretório e dentro dele um arquivo `Dockerfile` com os seguintes comandos:
  
    ```Dockerfile
    FROM ubuntu:latest
    RUN apt-get update && apt-get install -y curl
    ```

- Navegue até o diretório onde está o Dockerfile e execute o comando `docker build -t my-curl .`.
- Verifique se a imagem foi criada corretamente com `docker images`.

### 5. docker top
Lista os processos rodando dentro de um contêiner.

**Tarefa:**
- Execute um contêiner usando `docker run -d nginx`.
- Identifique o ID do contêiner usando `docker ps`.
- Use o comando `docker top <CONTAINER ID>` para listar os processos rodando dentro do contêiner.
- Observe a saída do comando.