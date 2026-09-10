# ☁️ Cloud Infrastructure Lab

Laboratório de infraestrutura em cloud desenvolvido para demonstrar práticas de **Infrastructure as Code (IaC)**, automação e organização de recursos utilizando **Terraform e AWS**.

O objetivo não é apenas provisionar recursos, mas demonstrar como estruturar uma infraestrutura de forma **reprodutível, organizada, segura e preparada para evolução**.

## 🎯 Objetivos

* Provisionar infraestrutura utilizando Terraform
* Aplicar princípios de Infrastructure as Code
* Organizar recursos por ambientes
* Utilizar variáveis, outputs e módulos
* Aplicar boas práticas de segurança
* Trabalhar com gerenciamento de estado
* Automatizar validações através de CI/CD
* Documentar decisões de arquitetura

## 🏗️ Arquitetura

A infraestrutura será composta por recursos como:

* VPC
* Subnets públicas e privadas
* Security Groups
* IAM
* EC2
* Load Balancer
* S3
* RDS
* CloudWatch

A arquitetura poderá evoluir conforme novos componentes forem adicionados ao laboratório.

## 🛠️ Tecnologias

* Terraform
* AWS
* Linux
* GitHub Actions
* Bash
* Python

## 📁 Estrutura

```text
.
├── environments/
│   ├── dev/
│   └── prod/
├── modules/
│   ├── network/
│   ├── compute/
│   ├── database/
│   └── security/
├── scripts/
├── .github/
│   └── workflows/
├── README.md
└── ...
```

## 🔄 Automação

O projeto utiliza pipeline para executar etapas como:

1. Formatação
2. Validação
3. Análise estática
4. Terraform Plan
5. Terraform Apply

O `apply` será controlado de acordo com o ambiente.

## 🔐 Segurança

O laboratório também considera práticas como:

* princípio do menor privilégio
* separação de ambientes
* gerenciamento adequado de secrets
* validação de infraestrutura
* análise de configuração

## 🧠 Decisões de arquitetura

Além do código, o projeto documenta algumas decisões e seus respectivos trade-offs.

A ideia é demonstrar não somente **como criar a infraestrutura**, mas também **por que determinadas decisões foram tomadas**.

> Este é um laboratório técnico e não representa necessariamente uma arquitetura pronta para produção.

## 🚀 Próximos passos

* Adicionar módulos reutilizáveis
* Implementar ambientes adicionais
* Integrar ferramentas de segurança
* Adicionar observabilidade
* Integrar deployment de uma aplicação
* Evoluir para uma arquitetura orientada a containers
