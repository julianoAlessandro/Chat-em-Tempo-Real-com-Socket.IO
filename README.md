
# 🌐 Deploy de Aplicação na AWS com Cloud9



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
- 🚀 **Deploy da aplicação** em um ambiente de execução na AWS.
- 🌐 Verificação de que a aplicação estava acessível via navegador.
- 📝 Documentação dos passos realizados em um `README.md`, incluindo:
  - Instruções de **Deploy**
  - Instruções de **Cleanup** (remoção dos recursos após uso)

---

## 🎯 Conclusão

A atividade proporcionou uma **experiência prática completa** de como preparar, adaptar e implantar uma aplicação na nuvem de forma organizada, seguindo **boas práticas de DevOps** e utilizando os recursos gratuitos fornecidos pela AWS por meio do ambiente educacional **Learner Lab**.
# 🚀 Deploy de Aplicação na AWS com Docker e Elastic Beanstalk

Este documento descreve passo a passo como foi realizado o deploy de uma aplicação Node.js utilizando Docker no ambiente da AWS, através do AWS Cloud9 e Elastic Beanstalk.

---

## 👨‍💻 Pré-requisitos

Antes de iniciar, certifique-se de que:

- Você possui uma conta AWS ativa.
- O ambiente **AWS Cloud9** está configurado e acessível.
- O repositório da aplicação foi clonado corretamente no Cloud9.

---

## ⚙️ Etapas do Deploy

### ✅ Passo 1 – Criar os arquivos do Docker

No diretório raiz da aplicação, crie os arquivos necessários para utilizar o Docker:

#### `Dockerfile`

```dockerfile
FROM node:18
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
CMD ["node", "server.js"]

### Exeucutando
- npm install
- eb init
- eb create nome-do-ambiente
- npm start
- CTRL + C encerrar servidor


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

