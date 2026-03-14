# Arquitetura da Solução AWS

## Visão Geral

A arquitetura proposta utiliza serviços gerenciados da AWS para garantir escalabilidade, alta disponibilidade e redução de custos operacionais.

A solução é composta pelos seguintes serviços:

- Amazon S3
- Amazon RDS
- AWS Lambda

Cada serviço possui uma função específica dentro da arquitetura do sistema da empresa.

---

## Componentes da Arquitetura

### Amazon S3

O Amazon S3 é utilizado como camada de armazenamento de objetos. Neste projeto, ele é responsável por armazenar documentos corporativos, relatórios, backups e registros relacionados às operações da empresa.

---

### Amazon RDS

O Amazon RDS é responsável por gerenciar o banco de dados relacional da aplicação. Ele armazena informações estruturadas, como dados de clientes, pedidos de medicamentos e controle de estoque.

---

### AWS Lambda

O AWS Lambda é utilizado para executar funções serverless responsáveis pelo processamento de dados do sistema, como processamento de pedidos, geração de relatórios e integração entre serviços.

---

## Fluxo da Aplicação

O fluxo da aplicação ocorre da seguinte forma:

1. Os usuários acessam o sistema da empresa para realizar pedidos ou consultas.
2. As requisições são processadas por funções AWS Lambda.
3. As funções Lambda interagem com o banco de dados hospedado no Amazon RDS.
4. Documentos e arquivos gerados pelo sistema são armazenados no Amazon S3.

---

## Benefícios da Arquitetura

A arquitetura proposta oferece diversos benefícios:

- Redução de custos com infraestrutura física
- Escalabilidade automática
- Alta disponibilidade
- Maior segurança no armazenamento de dados
