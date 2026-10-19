# Pedro Moraes

Desenvolvedor Python com foco em automação de processos, backend e arquitetura serverless na AWS. Trabalho do mapeamento do processo à sustentação em produção, integrando sistemas modernos e legados.

---

## Sobre

Atuo há mais de 3 anos com automação (RPA) e desenvolvimento de aplicações, em projetos que passam por backend, frontend, dados e infraestrutura.

- **Automação web e desktop:** robôs com Playwright, PyAutoGUI e Pywinauto, em operações de clientes como Bradesco, PagSeguro, Claro e iFood.
- **Sistemas legados:** integração com mainframe via TN3270 (py3270 / wc3270), sem depender de APIs.
- **Backend:** APIs REST com FastAPI e Django, com modelagem de dados relacional (PostgreSQL) e NoSQL (DynamoDB).
- **Cloud:** arquiteturas serverless na AWS, filas FIFO e workers em containers.
- **Dados:** queries SQL com CTEs, relatórios operacionais e dashboards.

---

## Projeto em destaque: plataforma de automação serverless

Plataforma fullstack para automação de processos, projetada e desenvolvida por mim de ponta a ponta, da modelagem de dados à infraestrutura. Conduzi também a migração completa de uma arquitetura em EC2 (Django + Angular) para uma arquitetura serverless.

**Arquitetura**

```
CloudFront ─┬─ S3 ............ frontend React
            └─ Lambda ........ API FastAPI (Mangum)
                  ├─ Cognito .. autenticação (JWT)
                  ├─ DynamoDB . dados
                  └─ SQS FIFO . filas de automação (com DLQ)
                        └─ Lambda (gatilho) ─► ECS Fargate ─► worker Playwright

EventBridge Scheduler ─► Lambda ─► enfileiramento de tarefas
```

**Experiência aplicada**

- Migração de Django + Angular + EC2 para FastAPI + React + Lambda, com modelagem orientada a padrões de acesso no DynamoDB.
- Processamento assíncrono com SQS FIFO, garantindo ordem por fluxo e tratamento de falhas com DLQ.
- Workers com Playwright em containers (ECR + Fargate), acionados por fila.
- Agendamento de rotinas com EventBridge Scheduler.
- Autenticação com Cognito e armazenamento de arquivos no S3.
- Controle de custos na AWS, como a troca do Secrets Manager pelo SSM Parameter Store.
- Logs e monitoramento no CloudWatch e permissões com IAM de menor privilégio.

---

## Stack

**Linguagens e frameworks**

[![Python](https://skillicons.dev/icons?i=python,fastapi,django,flask)](https://skillicons.dev)

**Frontend**

[![Frontend](https://skillicons.dev/icons?i=react,ts,js,html,css)](https://skillicons.dev)

**Dados e cloud**

[![Cloud](https://skillicons.dev/icons?i=aws,dynamodb,postgres,docker)](https://skillicons.dev)

**Ferramentas**

[![Tools](https://skillicons.dev/icons?i=linux,git,github)](https://skillicons.dev)

**AWS:** Lambda · CloudFront · S3 · DynamoDB · SQS (FIFO e DLQ) · EventBridge · ECS Fargate · ECR · Cognito · IAM · CloudWatch · SSM

**Automação e integração:** Playwright · PyAutoGUI · Pywinauto · py3270 / wc3270 · APIs REST · BPMN

---

## Contato

<div>
  <a href="mailto:pedrorms.contato@gmail.com"><img src="https://img.shields.io/badge/-Email-%23333?style=for-the-badge&logo=gmail&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/pedro-rodrigues-moraes-silveira-7b19783a0" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
</div>
