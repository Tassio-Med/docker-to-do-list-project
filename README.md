
# Bem-vindo ao repositório do projeto Docker Todo List!

Neste projeto temos uma aplicação full-stack, um **aplicativo de tarefas**! O objetivo foi conteinerizar a aplicação para ela poder funcionar.

Para isso foram desenvolvidos arquivos de configuração para cada frente específica: `Front-end` e `Back-end`. Também foram criadas imagens e configuradas com o `docker-compose`.

## Autores

- [@tassio_medeiros](https://github.com/Tassio-Med)

- [@trybe](https://github.com/betrybe)

É importante dar destaque que o projeto por completo não foi realizado por mim.
O `Front-end` e o `Back-end` foram construídos pela [@trybe](https://github.com/betrybe).

Fiquei responsável pela conteinerização aplicação, ou seja, tudo referente à `docker`.


## Uso/Exemplos

```docker
version: '3'
services:
  todofront:
    image: todofrontend
    ports:
      - 3000:3000
    depends_on:
      - todoback
    environment:
      - REACT_APP_API_HOST=todoback

  todoback:
    image: todobackend
    ports:
      - 3001:3001

```


## Referência

 - [Docker documentation](https://docs.docker.com/desktop/)
 - [Cheasheet for Docker CLI](https://github.com/matiassingers/awesome-readme)
 

