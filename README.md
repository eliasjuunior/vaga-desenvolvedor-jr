# DESENVOLVEDOR JR

## Demonstração

[![asciicast](docs/demonstracao.svg)]()

## Teste para a vaga de desenvolvedor Jr

Siga o passo a passo abaixo para a instalação e execução do código de teste para a vaga de desenvolvedor Jr.

### Detalhes do teste:

O código fonte desse teste está escrito em Ruby, usando um scaffold de uma app básica do framework Rails. O teste se baseia em instalar a aplicação e executa-lá em seu ambiente de desenvolvimento, escrever alguns testes que estão pendentes e corrigir outros conforme alerta do console.

### Após finalizar o teste



## Passos para instalação:

#### Requerimentos:

* Github
* Ruby >= 2.5
* Rails
* Terminal (Command prompt)

#### Conhecimentos necessários:

* Ruby
* Ruby on Rails
* RSPEC
* Git / Github
* Expressão regular (diferencial)

### 1. Clonar Repositório

  1.1 Para baixar o repositório, execute:
  ```bash
  $ git clone git@github.com:achievemore/vaga-desenvolvedor-jr.git
  ```

### 2. Fazer Build da Imagem Docker (ou executar da maneira que achar desejavel)

  2.1 Para entrar na pasta do projeto, digite:
  ```bash
  $ cd vaga-desenvolvedor-jr
  ```

  2.2 Para fazer a build da Imagem, execute:
  ```bash
  $ docker build -t achievemore-ruby .
  ```

### 3. Provisionamento do Rails

  3.1 Digite o comando abaixo, então tecle enter para criar um container e acessar o seu shell:
  ```bash
  $ docker run --rm -v `pwd`:/app -w /app -it achievemore-ruby /bin/sh
  ```

  3.2 Para criar as tabelas de teste, execute:
  ```bash
  $ bundle exec rails db:migrate
  ```

### 4. Rodar os Testes

  4.1 Agora rode os testes da seguinte forma:
  ```bash
  $ bundle exec rspec
  ```
