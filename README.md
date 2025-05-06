# Desafio Final - Pipeline e Deploy de Aplicação Simples

Este repositório contém a implementação de um pipeline de **build** e **deploy** de uma aplicação simples. O objetivo é demonstrar a criação de um pipeline utilizando o **GitHub Actions** para automatizar o processo de deploy de uma aplicação estática (HTML).

## Estrutura do Projeto

A estrutura do projeto é bem simples:

PROJETO_FINAL/
│
├── index.html # Página principal da aplicação
├── .github/ # Diretório para workflows do GitHub Actions
│ └── workflows/
│ └── pipelines.yml # Arquivo de configuração do GitHub Actions para build e deploy
├── README.md # Este arquivo
└── .gitignore # Arquivo para ignorar arquivos não rastreados


## Funcionalidade

O **pipeline** automatiza os seguintes passos:

1. **Verificação de existência do `index.html`:** O pipeline verifica se o arquivo `index.html` existe no repositório.
2. **Deploy para GitHub Pages:** Caso o arquivo `index.html` esteja presente, o pipeline realiza o deploy da aplicação para o GitHub Pages. O deploy é feito na branch `gh-pages`, garantindo que o conteúdo da aplicação está disponível online.

## Como Usar

1. **Clonar o repositório:**

   Para clonar o repositório em seu ambiente local, execute:

   ```bash
   git clone https://github.com/seu_usuario/desafio_final.git
   cd desafio_final
