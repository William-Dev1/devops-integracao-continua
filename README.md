# DevOps e Integração Contínua

Projeto acadêmico desenvolvido para a disciplina de
DevOps e Integração Contínua.

## Descrição

Este projeto demonstra a aplicação de práticas DevOps
em uma aplicação web simples desenvolvida para a
empresa fictícia CodeFactory Solutions.

Durante o desenvolvimento são utilizados controle de
versão, branches, Pull Requests, containers e
Integração Contínua.

## Objetivo

Demonstrar como práticas DevOps podem tornar o
desenvolvimento de software mais organizado,
colaborativo, automatizado e confiável.

## Tecnologias utilizadas

- HTML
- CSS
- JavaScript
- Git
- GitHub
- Docker
- GitHub Actions

## Estrutura do projeto

```text
devops-integracao-continua/
├── .github/
│   └── workflows/
│       └── ci.yml
├── src/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── Dockerfile
├── .dockerignore
├── README.md
└── LICENSE
```

## Instalação

Clone o repositório:

```bash
git clone https://github.com/William-Dev1/devops-integracao-continua.git
```

Entre na pasta:

```bash
cd devops-integracao-continua
```

## Execução com Docker

Construa a imagem:

```bash
docker build -t devops-integracao-continua .
```

Execute o container:

```bash
docker run -d -p 8080:80 --name devops-app devops-integracao-continua
```

Abra no navegador:

```text
http://localhost:8080
```

## Estratégia de branches

O projeto utiliza três branches principais:

- main
- desenvolvimento
- features

## Integração Contínua

A Integração Contínua é realizada através do
GitHub Actions.

A pipeline verifica os arquivos da aplicação,
constrói uma imagem Docker, inicia o container
e realiza um teste de acesso à aplicação.

## Licença

Este projeto utiliza a licença MIT.