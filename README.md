# Githubactions_pipeline

Fala pessoal, tudo certo ? Espero que sim. Hoje eu venho compartilhar este repositório, que consiste em um pequeno lab, de como automatizar a etapa de CI de uma aplicação, através de um **pipeline** no **GithubActions**.
A pipeline em si, tem como objetivo realizar testes em um aplicação nesta aplicação em **Go**, que se trata de uma API, que realize algumas consultas em um banco **Postgres**. Toda a aplicação, esta sendo conteinerizada através do **Docker**, e segue os seguintes passos para execução:

`Setar a versão do GO > Buildar a imagem do banco > Criar o banco > Testar a aplicação > Buildar a aplicação`

Estas tarefas, estão separadas em dois jobs, sendo um deles o job de **test**, e o outro de **build**. A pipeline se encontra na pasta `.github/workflows`, no arquivo em específico chamado **go.yaml**.
