# Projeto Docker Aquecimento

Este projeto é um exemplo básico de como criar e configurar um contêiner Docker utilizando a imagem base do Ubuntu 22.04. Ele demonstra a criação de um diretório simples dentro do contêiner.

## Estrutura do Projeto

- **Dockerfile**: Contém as instruções para construir a imagem Docker.

## Conteúdo do Dockerfile

O `Dockerfile` utiliza a imagem base do Ubuntu 22.04 e executa o seguinte comando:

```dockerfile
FROM ubuntu:22.04
RUN mkdir teste2
```

### Explicação dos comandos:

1. **`FROM ubuntu:22.04`**: Define a imagem base como Ubuntu 22.04.
2. **`RUN mkdir teste2`**: Cria um diretório chamado `teste2` dentro do contêiner.

## Como Usar o Docker

### Pré-requisitos

- Certifique-se de que o Docker está instalado em sua máquina. Para instalar, siga as instruções no site oficial: [Docker Documentation](https://docs.docker.com/get-docker/).

### Passos para Construir e Executar o Contêiner

1. **Construir a Imagem Docker**:

   No terminal, navegue até o diretório onde o `Dockerfile` está localizado e execute o seguinte comando:

   ```bash
   docker build -t docker-aquecimento .
   ```

   Este comando cria uma imagem Docker chamada `docker-aquecimento`.

2. **Executar o Contêiner**:

   Após construir a imagem, execute o seguinte comando para iniciar o contêiner:

   ```bash
   docker run -it docker-aquecimento
   ```

   O contêiner será iniciado e você estará dentro dele.

3. **Verificar o Diretório Criado**:

   Dentro do contêiner, execute o comando abaixo para verificar se o diretório `teste2` foi criado:

   ```bash
   ls
   ```

   Você verá o diretório `teste2` listado.

## Contribuição

Sinta-se à vontade para contribuir com melhorias ou sugestões para este projeto.

## Licença

Este projeto está sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.