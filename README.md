# 🚀 Automação Inteligente de Onboarding de Clientes com n8n

Uma automação desenvolvida utilizando **n8n**, **Google Forms**, **Google Sheets**, **Google Gemini (IA)** e **Gmail**, com o objetivo de automatizar o processo de recepção e relacionamento com novos clientes e clientes já existentes.

> Este projeto foi desenvolvido do zero, utilizando lógica de automação, integrações entre serviços e agentes de Inteligência Artificial para reduzir tarefas manuais e oferecer um atendimento mais rápido, inteligente e personalizado.

---

# 📌 O Problema

Empresas recebem diversas respostas de formulários diariamente e, muitas vezes, precisam analisar manualmente cada cliente para decidir qual abordagem utilizar.

Esse processo costuma gerar:

- Tempo perdido com tarefas repetitivas;
- Demora no primeiro contato;
- Atendimento pouco personalizado;
- Maior chance de erros humanos;
- Sobrecarga operacional.

---

# 💡 A Solução

Este workflow automatiza completamente esse processo.

Sempre que um cliente responde ao formulário:

- Os dados são registrados automaticamente no Google Sheets;
- O n8n identifica uma nova resposta;
- O workflow analisa se o cliente é novo ou já possui relacionamento com a empresa;
- Um agente de IA gera uma mensagem personalizada;
- O sistema envia automaticamente um e-mail adequado ao perfil daquele cliente.

Todo esse fluxo acontece sem qualquer intervenção humana.

---

# ⚙️ Como Funciona

## 1. Recebimento do formulário

O cliente preenche um formulário no Google Forms.

↓

## 2. Armazenamento dos dados

As respostas são enviadas automaticamente para uma planilha do Google Sheets.

↓

## 3. Monitoramento

O Google Sheets Trigger do n8n monitora continuamente a planilha.

Quando uma nova linha é adicionada, o workflow é iniciado automaticamente.

↓

## 4. Análise do cliente

Uma condicional (IF) verifica:

- Cliente novo
- Cliente já existente

↓

## 5. Geração da resposta com IA

### Cliente Novo

O agente de IA:

- Analisa as respostas;
- Cria uma mensagem de boas-vindas;
- Explica os serviços oferecidos;
- Apresenta a empresa de forma personalizada;
- Finaliza com uma proposta comercial leve.

### Cliente Existente

O agente de IA:

- Analisa o histórico informado;
- Avalia o feedback recebido;
- Agradece clientes satisfeitos;
- Pede desculpas quando necessário;
- Gera uma proposta comercial personalizada para continuidade dos serviços.

↓

## 6. Envio automático

O Gmail envia automaticamente o e-mail gerado pela IA para o cliente.

---

# 🧠 Tecnologias Utilizadas

- n8n
- Google Forms
- Google Sheets
- Google Gemini AI
- Gmail API
- IA Generativa
- Workflows
- Automação de Processos
- Lógica Condicional
- HTML para formatação de e-mails

---

# 🔄 Fluxograma

```text
Google Forms
      │
      ▼
Google Sheets
      │
      ▼
Google Sheets Trigger (n8n)
      │
      ▼
IF (Cliente Novo?)
      │
 ┌────┴────┐
 │         │
 ▼         ▼
Cliente   Cliente
 Novo     Existente
 │         │
 ▼         ▼
Agente IA Agente IA
 │         │
 ▼         ▼
Mensagem  Proposta Comercial
 │         │
 └────┬────┘
      ▼
 Gmail
      │
      ▼
Cliente recebe o e-mail automaticamente
```

---

# 🚀 Funcionalidades

- Monitoramento automático de formulários
- Integração entre Google Forms e Google Sheets
- Execução automática via Trigger
- Condicionais inteligentes
- Personalização utilizando Inteligência Artificial
- Envio automático de e-mails
- Atendimento personalizado
- Processo totalmente automatizado

---

# 📈 Benefícios

- Redução de tarefas manuais
- Atendimento imediato
- Escalabilidade
- Padronização das respostas
- Melhor experiência para o cliente
- Economia de tempo operacional

---

# 🔧 Como Reproduzir

## Pré-requisitos

- n8n instalado (Cloud ou Self-hosted)
- Conta Google
- Google Forms
- Google Sheets
- Credenciais do Google configuradas
- Credenciais do Gmail
- API do Google Gemini configurada

## Passos

1. Clone este repositório.
2. Importe o arquivo `.json` no n8n.
3. Configure suas credenciais do Google.
4. Configure suas credenciais do Gmail.
5. Configure sua API do Google Gemini.
6. Substitua a planilha e o formulário pelos seus.
7. Execute um teste enviando uma resposta ao formulário.

---

# 📚 Aprendizados

Durante o desenvolvimento deste projeto foram aplicados conceitos como:

- Integração entre APIs
- Automação de processos
- Desenvolvimento de Workflows
- Engenharia de Prompts
- Agentes de Inteligência Artificial
- Processamento de dados
- Fluxos condicionais
- Boas práticas em automação

---

# 📸 Demonstração

Adicione aqui:

- Screenshot do Workflow
- Screenshot da execução
- Screenshot dos e-mails gerados
- GIF ou vídeo demonstrando o funcionamento

---

# 👨‍💻 Autor

**Lucas Braun**

Estudante de Automação Industrial | Desenvolvedor de Automações com n8n | Entusiasta de Inteligência Artificial e Automação de Processos.

Sempre em busca de criar soluções inteligentes que economizem tempo, aumentem a produtividade e gerem valor para empresas através da tecnologia.

---

## ⭐ Se este projeto foi útil para você

Considere deixar uma ⭐ no repositório para apoiar o projeto.
