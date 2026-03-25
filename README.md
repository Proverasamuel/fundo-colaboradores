# 💰 Sistema de Gestão de Fundo Financeiro

Plataforma web desenvolvida para gestão de um fundo financeiro colaborativo, permitindo o controle de **depósitos, empréstimos e levantamentos**, com validação por moderadores e acompanhamento em tempo real pelos usuários.

---

## 📌 Visão Geral

O sistema foi criado para digitalizar e otimizar a gestão de fundos financeiros em organizações, garantindo:

* Transparência nas operações
* Controle eficiente de solicitações
* Segurança no acesso e nas transações
* Melhor experiência para usuários e administradores

---

## 🚀 Funcionalidades

### 👤 Usuários

* Cadastro e autenticação segura
* Visualização do saldo atualizado
* Solicitação de:

  * Levantamentos
  * Empréstimos
* Acompanhamento do status das solicitações

### 💼 Moderadores

* Validação de depósitos enviados pelos usuários
* Registro manual de depósitos (com comprovativo)
* Aprovação ou rejeição de:

  * Levantamentos
  * Empréstimos

### 💳 Operações

* Depósitos tratados como **operações diretas**
* Levantamentos e empréstimos tratados como **solicitações com fluxo de aprovação**
* Atualização automática do saldo após validação

---

## 🛠️ Tecnologias Utilizadas

### Backend

* **Laravel**
* **MySQL**
* **Laratrust** (controle de roles e permissões)
* **Laravel Sanctum** (autenticação)

### Frontend

* **Angular**
* **Tailwind CSS**

---

## 🧠 Arquitetura

O sistema segue uma arquitetura baseada em **API REST**, com separação clara entre frontend e backend:

* Backend responsável pela lógica de negócio e segurança
* Frontend responsável pela interface e experiência do usuário

---

## 🔐 Segurança

* Autenticação baseada em tokens (Sanctum)
* Controle de acesso baseado em roles (Laratrust)
* Validação de operações críticas por moderadores
* Proteção contra acessos não autorizados

---


## ⚙️ Como Executar o Projeto

### 🔧 Backend (Laravel)

```bash
git clone https://github.com/Proverasamuel/fundo-colaboradores.git
cd fundo-financeiro

composer install

cp .env.example .env
php artisan key:generate

# Configurar banco de dados no .env

php artisan migrate
php artisan serve
```

---

### 🌐 Frontend (Angular)

```bash
cd frontend

npm install

ng serve
```

Acesse:

```
http://localhost:4200
```

---

## 🔄 Fluxo de Funcionamento

1. Usuário realiza depósito via banco ou Multicaixa Express
2. Envia comprovativo
3. Moderador valida e registra o depósito
4. Saldo é atualizado automaticamente
5. Usuário pode solicitar levantamento ou empréstimo
6. Moderador aprova ou rejeita a solicitação

---

## 📈 Melhorias Futuras

* Integração com APIs de pagamento (Multicaixa Express)
* Notificações em tempo real
* Dashboard analítico
* Histórico detalhado de transações
* Sistema de auditoria

---

## 👨‍💻 Autor

**Provera Samuel**
Desenvolvedor Web | Backend & Frontend

* GitHub: [https://github.com/Proverasamuel](https://github.com/Proverasamuel)
* LinkedIn: *https://www.linkedin.com/in/prover%C3%A1-samuel/*

---

## 📄 Licença

Este projeto está sob a licença MIT.

---

## ⭐ Considerações Finais

Este projeto demonstra habilidades em:

* Desenvolvimento de APIs REST
* Controle de permissões e autenticação
* Modelagem de sistemas financeiros
* Integração entre frontend e backend
* Boas práticas de arquitetura de software


