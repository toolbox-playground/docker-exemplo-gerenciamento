# docker-exemplo-gerenciamento

Esse repositório oferece exercícios práticos para ter um bom gerenciamento em Docker

## Estrutura do repositório
```
|__.github                          # Pasta com os arquivos de CI/CD para o GitHub Actions
|__exercicios                       # Exercícios 
|  |__1-... 
|  |  |__Dockerfile                    # Arquivo principal para execução do Docker
|  |__2-...                          
|__CHANGELOG.md                     # Arquivo de controle de changes do repositório
|__CONTRIBUTING.md                  # Arquivo com diretrizes de contribuição
|__package.json                     # Arquivo necessário para geração de versionamento automático
|__README.md                        # Você está lendo esse arquivo
|__.versionrc                       # Arquivo necessário para configuração de versionamento
```

## Pré-requesito
## 1. Baixar o Docker Desktop
Abra seu navegador web e acesse a página oficial de download do Docker. Baixe o Docker Desktop de acordo com o seu sistema operacional.
Faça o download aqui → [Docker Desktop)](https://www.docker.com/products/docker-desktop/)

## 2. Executar o Instalador

1. Após o download, execute o arquivo 

   ```Docker Desktop Installer.exe```

2. Siga as instruções do instalador. Quando a instalação for concluida, clique em "Close"

## 3. Finalizando a Instalação do Docker Desktop

1. Após a instalação do Docker Desktop, procure por Docker e selecione "Docker Desktop" para abrir a ferramenta

2. Durante a primeira execução, será solicitado para fazer login ou criar uma conta Docker.

## 4. Verificação da Instalação

1. Abra o terminal PowerShell (Terminal).

2. Execute o comando para verificar a versão do Docker instalada:

   ```docker --version```

   Você deve ver uma saída semelhante a:

    ```Docker version 20.10.8, build 3967b7d```

## 5. Testando o Docker

1. No terminal, execute o comando para rodar um container de teste:

   ```docker run hello-world```

   Este comando faz o download de uma imagem de teste do Docker Hub e executa um container que imprime uma mensagem de "Hello from Docker!".

## 6. Verificação do Docker Engine

1. Execute o comando abaixo para listar todos os containers ativos. Se não houver containers rodando, retornará uma lista vazia:

   ```docker ps```

2. Execute o comando abaixo para listar todos os contêineres, incluindo os que estão parados:

    ```docker ps -a```
