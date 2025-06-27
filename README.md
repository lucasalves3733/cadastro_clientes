# 📋 Cadastro de Clientes

Sistema completo de cadastro de clientes com **React.js** no frontend e **Node.js + MySQL** no backend.

O projeto possui a seguinte estrutura de pastas:

cadastro_clientes/
backend/ # API Node.js com Express e MySQL
frontend/ # Aplicação React com Material-UI
README.md # Arquivo de documentação

markdown
Copiar
Editar

## 🛠 Tecnologias Utilizadas

**Frontend**
- React.js
- Material-UI
- Axios

**Backend**
- Node.js
- Express
- MySQL
- CORS
- Body-Parser

**Banco de Dados**
- MySQL

## ✨ Funcionalidades

✅ Cadastro de clientes  
✅ Edição de clientes  
✅ Exclusão de clientes  
✅ Listagem dos clientes em uma tabela  
✅ API RESTful completa para integração com o frontend

## 🚀 Como Rodar Localmente

### 📋 Pré-requisitos

Certifique-se de ter instalado:
- Node.js
- MySQL
- Git

### 🗄 Configuração do Banco de Dados

**Passo 1:** Criação do banco de dados

```sql
CREATE DATABASE cadastro_clientes;
Passo 2: Seleção do banco

sql
Copiar
Editar
USE cadastro_clientes;
Passo 3: Criação da tabela clientes

sql
Copiar
Editar
CREATE TABLE IF NOT EXISTS clientes (
  id INT AUTO_INCREMENT PRIMARY KEY,
  nome VARCHAR(100) NOT NULL,
  email VARCHAR(100) NOT NULL,
  telefone VARCHAR(20) NOT NULL,
  endereco VARCHAR(200) NOT NULL
);
⚙️ Configuração do Backend
Acesse a pasta:

bash
Copiar
Editar
cd backend
Instale as dependências:

nginx
Copiar
Editar
npm install
Configure a conexão com o MySQL em index.js:

javascript
Copiar
Editar
const db = mysql.createPool({
  host: 'localhost',
  user: 'root',
  password: 'SUA_SENHA',
  database: 'cadastro_clientes'
});
Inicie o servidor:

nginx
Copiar
Editar
node index.js
Backend ficará disponível em: http://localhost:3001

💻 Configuração do Frontend
Acesse a pasta:

bash
Copiar
Editar
cd frontend
Instale as dependências:

nginx
Copiar
Editar
npm install
Ajuste o endpoint da API em App.js, se necessário:

javascript
Copiar
Editar
const apiURL = 'http://localhost:3001/clientes';
Inicie o frontend:

sql
Copiar
Editar
npm start
Frontend ficará disponível em: http://localhost:3000

🌐 Deploy
O projeto está pronto para deploy:

Backend: Railway, Render, ou Heroku.

Frontend: Netlify ou Vercel.

👤 Autor
Projeto desenvolvido por Lucas Alves.

📄 Licença
Este projeto é open-source e pode ser utilizado para fins acadêmicos.

