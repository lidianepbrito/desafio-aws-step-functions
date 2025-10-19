
# 🚀 Desafio AWS Step Functions - DIO

## 🧭 Sobre o Desafio
Este projeto foi desenvolvido como parte do **laboratório prático da DIO**, com o objetivo de consolidar os conhecimentos adquiridos sobre **AWS Step Functions** e **integração com AWS Lambda**.  

O foco foi criar e compreender fluxos automatizados (workflows) que orquestram funções em nuvem, aplicando validações, lógica condicional e automação de processos.

---

## 🧩 Tópicos Estudados

### 1️⃣ Conhecendo o AWS Step Functions
- Entendimento do conceito de **orquestração de serviços**.
- Estudo sobre **máquinas de estado (State Machines)** e como elas controlam o fluxo de execução.
- Diferença entre **Step Functions Standard e Express**.
- Introdução à **interface visual** da AWS para criação de workflows.

### 2️⃣ Benefícios e Projeto Modelo no AWS Step Functions
- Identificação dos principais **benefícios**: automação, escalabilidade, visibilidade e baixo acoplamento.
- Construção de um **projeto modelo** usando o **Amazon States Language (ASL)**.
- Integração com outros serviços AWS (Lambda, SNS e SQS).

### 3️⃣ Realizando Validações no AWS Step Functions
- Criação de **condições de decisão** com estados do tipo *Choice*.
- Uso de **validações de entrada e saída**.
- Testes de fluxos com diferentes cenários (sucesso e falha).
- Aplicação de boas práticas de monitoramento e logs com o **CloudWatch**.

### 4️⃣ Criando e Executando Lambda no AWS Step Functions
- Criação de funções Lambda em Python.
- Integração direta da **Lambda Function** no workflow.
- Testes práticos de execução (startExecution).
- Tratamento de **erros e exceções**.

## 🧠 Aprendizados e Insights

Durante o desafio, aprimorei minha compreensão sobre como:

- Automatizar tarefas com **fluxos de decisão inteligentes**;
- Integrar **múltiplos serviços AWS** em um só processo;
- Documentar de forma técnica e estruturada;
- Utilizar o **GitHub como portfólio profissional**.

💬 Conclusão👀,📚

Projeto concluído com sucesso! 🎯
Durante o desafio AWS Step Functions, pude aplicar os conceitos abordados, explorando desde o funcionamento das máquinas de estado até a integração com funções Lambda.
Com isso, compreendi como os workflows automatizados orquestram diferentes serviços da AWS com eficiência, escalabilidade e controle.

Graças a Deus, tudo ocorreu bem 🙏 e o aprendizado foi muito enriquecedor.
Mais tenho que colocar em prática, pois ainda tenho muita caminhada pela frente. 💻✨


---

## ⚙️ Arquitetura Simplificada do Projeto

```mermaid
graph TD
A[Início] --> B[Validação de Entrada]
B -->|Validação OK| C[Executa Função Lambda]
B -->|Erro| D[Fim com Erro]
C --> E[Registro no CloudWatch]
E --> F[Fim com Sucesso]



