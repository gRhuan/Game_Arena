# Campeonato de FIFA - Sistema de Inscrição

Sistema web para gerenciamento de inscrições de campeonato de FIFA.

---

## 📌 Tecnologias Utilizadas

- **Backend**: JAVA SPRING BOOT  
- **Banco de Dados**: MySQL  
- **Servidor**: NGINX  
- **Frontend**: HTML + CSS + JavaScript  

---

## ✅ Funcionalidades obrigatórias

### 1. Página principal
- Nome do site e breve descrição sobre o campeonato de FIFA.
- Formulário de inscrição.
- Utilização da paleta de cores da Unifucamp.

### 2. Formulário de inscrição
Campos obrigatórios:
- Nome completo do jogador
- Nickname (nome de jogador)
- E-mail para contato
- Idade
- Upload do comprovante de pagamento da inscrição
- Termos e condições (checkbox para aceitar)

### 3. Validação dos dados
- Validação básica dos campos obrigatórios usando PHP.
- Validação do pagamento será feita **manualmente**.
- Envio de e-mail ao participante confirmando a inscrição.

### 4. Armazenamento dos dados
- As inscrições devem ser salvas em uma tabela `inscricoes` no MySQL.
- Tabela deve conter todos os campos mencionados no formulário.

### 5. Página de administração (simples)
- Listagem de todos os inscritos.
- Exibição dos dados em uma tabela HTML com informações do banco.

---

## 🔧 Tarefas por área

### 🔙 Backend (JAVA)
- Criar lógica para:
  - Validação dos dados do formulário.
  - Upload e salvamento do comprovante.
- Integração com banco de dados (salvar e listar inscritos).
- Criar endpoint ou página para administração (exibir inscritos).

### 🗃️ DBA (MySQL)
- Criar banco de dados com uma tabela chamada `inscricoes`.
- Campos sugeridos:
  - `id` (INT, AUTO_INCREMENT)
  - `nome_completo` (VARCHAR)
  - `nickname` (VARCHAR)
  - `email` (VARCHAR)
  - `idade` (INT)
  - `comprovante_pagamento` (VARCHAR ou TEXT, para caminho do arquivo)
  - `aceitou_termos` (BOOLEAN)
  - `data_inscricao` (DATETIME)

### 🎨 Frontend (HTML + CSS + JS)
- Criar a página principal com:
  - Layout responsivo e acessível.
  - Formulário estilizado (cores da Unifucamp).
  - Interações básicas (ex: validação de campos com JS, mensagens de erro).
- Criar página de administração simples com uma tabela HTML para mostrar os dados dos inscritos.

---

## 🚀 Como rodar o projeto

1. Clonar o repositório
```bash
git clone https://github.com/dieg0x20/Game_Arena.git
