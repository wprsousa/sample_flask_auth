<file name=0 path=README.md># Sample Flask Auth

Um projeto simples de autenticação com Flask, utilizando Flask-Login e SQLite. Ideal para aprender como funciona o fluxo de login, logout, registro e rotas protegidas em uma aplicação web com Flask.

---

## 🚀 Tecnologias

- Python 3.x  
- Flask  
- Flask-Login  
- SQLAlchemy  
- SQLite
- bcrypt

---

## 📦 Funcionalidades

- Cadastro de usuário com senha criptografada  
- Login e logout  
- Sessão de usuário com Flask-Login  
- Rotas protegidas  


---

## 🔧 Instalação

```bash
# Clone o repositório
git clone https://github.com/wprsousa/sample_flask_auth.git
cd sample_flask_auth

# Crie o ambiente virtual
python -m venv venv

# Ative o ambiente virtual
source venv/bin/activate        # Linux/Mac
venv\Scripts\activate         # Windows

# Instale as dependências
pip install -r requirements.txt
```

---

## ⚙️ Configuração

### Variáveis de ambiente

```bash
# Linux/Mac
export FLASK_APP=run.py
export FLASK_ENV=development

# Windows (CMD)
set FLASK_APP=run.py
set FLASK_ENV=development
```

### Inicialize o banco de dados

```bash
flask shell
>>> from app import db
>>> db.create_all()
>>> db.session.commit()
>>> exit()
```

---

## ▶️ Executando o Projeto

```bash
flask run
```

Acesse no navegador:  
[http://localhost:5000](http://localhost:5000)

A API também pode ser testada via ferramentas como Postman ou cURL. Por exemplo, para criar um usuário:

```bash
curl -X POST http://localhost:5000/user \
-H "Content-Type: application/json" \
-d '{"username": "admin", "password": "123"}'
```

---

## 🗂 Estrutura de Pastas

```
sample_flask_auth/
├── app.py
├── models/
│   └── user.py
├── database.py
├── requirements.txt
└── venv/
```

---

## 🧪 Rotas

- `POST /login` – Faz login do usuário  
- `GET /logout` – Faz logout do usuário autenticado  
- `POST /user` – Cria um novo usuário  
- `GET /user/<int:id_user>` – Retorna dados de um usuário específico (requer autenticação)  
- `PUT /user/<int:id_user>` – Atualiza a senha de um usuário específico (requer autenticação – apenas o próprio usuário ou perfis não‑"user")  
- `DELETE /user/<int:id_user>` – Deleta um usuário específico (requer autenticação – somente admin, não pode deletar a si mesmo)  


---

## 🙋 Contato

Desenvolvido por [@wprsousa](https://github.com/wprsousa)
</file>
