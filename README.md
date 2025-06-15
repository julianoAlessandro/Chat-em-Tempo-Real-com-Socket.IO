
# 🌐 Deploy de Aplicação na AWS com Cloud9

## 👥 Integrantes da Atividade

1. Gabriel Almir  
2. Gustavo  
3. Celso  
4. Pamela  
5. Juliano  

---

## 📘 Atividade Avaliativa Final – Deploy de Aplicação no AWS Learner Lab

Esta atividade avaliativa teve como objetivo principal a realização do **deploy de uma aplicação na nuvem utilizando os recursos do AWS Learner Lab**, com foco no desenvolvimento de habilidades práticas em computação em nuvem.

O processo iniciou-se com a **clonagem de um repositório já existente no GitHub para um repositório pessoal do aluno**, permitindo que as modificações necessárias fossem realizadas com base nos requisitos da AWS. Esse repositório continha o **código-fonte da aplicação**, que foi adaptado para ser compatível com os serviços de infraestrutura da AWS.

---

## ☁️ Serviços Utilizados

O principal serviço da AWS utilizado durante a atividade foi o **AWS Cloud9**, um ambiente de desenvolvimento integrado (IDE) baseado na nuvem, que permitiu aos integrantes:

- Editar o código-fonte da aplicação.
- Instalar dependências.
- Configurar o ambiente.
- Executar comandos diretamente em um terminal Linux na nuvem.

O **Cloud9 também funcionou como ambiente local na nuvem**, facilitando toda a preparação da aplicação para o processo de deploy.

---

## ⚙️ Etapas Realizadas

A partir do AWS Cloud9, as seguintes práticas foram executadas:

- 📦 **Configuração da infraestrutura como código (IaC)**, utilizando serviços como:
  - AWS Elastic Beanstalk
  - Amazon EC2
  - Amazon S3
- 🚀 **Deploy da aplicação** em um ambiente de execução na AWS.
- 🌐 Verificação de que a aplicação estava acessível via navegador.
- 📝 Documentação dos passos realizados em um `README.md`, incluindo:
  - Instruções de **Deploy**
  - Instruções de **Cleanup** (remoção dos recursos após uso)

---

## 🎯 Conclusão

A atividade proporcionou uma **experiência prática completa** de como preparar, adaptar e implantar uma aplicação na nuvem de forma organizada, seguindo **boas práticas de DevOps** e utilizando os recursos gratuitos fornecidos pela AWS por meio do ambiente educacional **Learner Lab**.

---

## 📁 Estrutura Recomendada do Repositório

```bash
├── .elasticbeanstalk/
├── app/
│   └── index.js
├── .gitignore
├── package.json
├── README.md  ← este arquivo
└── template.yaml  ← (opcional) IaC com AWS SAM ou CloudFormation


# socket.io

[![Latest NPM version](https://img.shields.io/npm/v/socket.io.svg)](https://www.npmjs.com/package/socket.io)
[![Build status](https://github.com/socketio/socket.io/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/socketio/socket.io/actions/workflows/ci.yml)
[![Downloads per month](https://img.shields.io/npm/dm/socket.io.svg)]((https://www.npmjs.com/package/socket.io))


## License

[MIT](https://opensource.org/licenses/MIT)
