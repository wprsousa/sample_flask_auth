# Sample Flask Auth

Um projeto simples de autenticação com Flask, utilizando Flask-Login e SQLite. Ideal para aprender como funciona o fluxo de login, logout, registro e rotas protegidas em uma aplicação web com Flask.

---

## 🚀 Tecnologias

- Python 3.x  
- Flask  
- Flask-Login  
- SQLAlchemy  
- SQLite  
- Bootstrap 5 (via CDN)

---

## 📦 Funcionalidades

- Cadastro de usuário  
- Login e logout  
- Sessão de usuário com Flask-Login  
- Rotas protegidas  
- Dashboard privado  
- Estrutura de templates com Jinja2

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
>>> exit()
```

---

## ▶️ Executando o Projeto

```bash
flask run
```

Acesse no navegador:  
[http://localhost:5000](http://localhost:5000)

---

## 🗂 Estrutura de Pastas

```
sample_flask_auth/
├── app/
│   ├── static/
│   ├── templates/
│   ├── config.py
│   ├── forms.py
│   ├── models.py
│   └── views.py
├── run.py
└── requirements.txt
```

---

## 🧪 Rotas

- `/` – Página inicial  
- `/login` – Tela de login  
- `/register` – Tela de cadastro  
- `/dashboard` – Página protegida  
- `/logout` – Logout

---

## 📄 Licença

Este projeto está licenciado sob a licença MIT.  
Consulte o arquivo `LICENSE.md` para mais detalhes.

---

## 🙋 Contato

Desenvolvido por [@wprsousa](https://github.com/wprsousa)  
Contribuições e feedbacks são bem-vindos!
