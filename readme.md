# 🧩 Projeto_7_Validação_de_Login_com_Flask

---

## 🚀 Descrição do Projeto

O **Projeto 9 - Validação de Login com Flask** tem como objetivo demonstrar o funcionamento de um sistema simples de autenticação de usuários utilizando o **framework Flask**, com foco em **rotas, formulários, segurança de senhas e persistência de dados**.

O usuário pode **cadastrar uma nova conta** e **realizar login** com verificação segura de senha.

---

## 🎯 Situação-Problema

Você foi contratado por uma pequena empresa que precisa de um **sistema de login seguro** para seus colaboradores acessarem uma área restrita.  
A empresa deseja uma solução simples, local e educativa, onde os dados dos usuários sejam salvos em um arquivo JSON.

Seu desafio é desenvolver uma aplicação Flask com:
- Rota de cadastro (`/register`)
- Rota de login (`/login`)
- Validação segura de senha
- Interface HTML funcional e responsiva

---

## 🧠 Objetivos de Aprendizagem

- Criar rotas com **Flask**
- Manipular formulários HTML usando **métodos GET e POST**
- Aplicar **hashing de senhas** com `werkzeug.security`
- Armazenar e ler usuários a partir de um **arquivo JSON**
- Exibir mensagens condicionais (“Acesso Permitido” / “Acesso Negado”)
- Integrar o back-end Flask a um front-end HTML responsivo

---

## ⚙️ Tecnologias Utilizadas

- **Python 3**
- **Flask**
- **Werkzeug**
- **HTML5** e **CSS3** (layout base disponibilizado por [html5up.net](https://html5up.net))
- **JSON** (para armazenamento local dos usuários)

---

## 🧩 Estrutura de Arquivos
```bash
Projeto_9_Validação_de_Login_com_Flask/
│
├── templates/
│ ├── login.html
│ └── cadastrar.html
│
├── usuarios.json
│
└── app.py
```


---

## 🔐 Principais Funcionalidades

- **Cadastro de novos usuários:**  
  Os dados são enviados via formulário HTML e armazenados no arquivo `usuarios.json`.

- **Validação de senha com hash:**  
  O sistema não armazena senhas em texto puro.  
  Utiliza as funções:
  ```python
  from werkzeug.security import generate_password_hash, check_password_hash
    ```

- **Para gerar e verificar o hash de cada senha.**
Login seguro:
Ao tentar logar, o sistema verifica o e-mail e a senha informados, exibindo:
- ✅ “Acesso Permitido” se o login for válido;
- ❌ “Acesso Negado” se o e-mail não existir ou a senha estiver incorreta.

---

# 💡 Exemplo de Uso

- Acesse a rota /register para criar uma conta.
- Preencha o e-mail e senha e clique em “Cadastrar”.
- Vá até /login e entre com os mesmos dados.
- O sistema exibirá uma mensagem indicando se o acesso foi permitido.

---

# 📘 Conceitos Trabalhados

| Conceito                  | Descrição                                            |
| ------------------------- | ---------------------------------------------------- |
| **Rotas Flask**           | Definição de URLs e suas funções correspondentes.    |
| **Métodos GET e POST**    | Envio e recepção de dados de formulários HTML.       |
| **Hashing de senhas**     | Segurança por meio de criptografia unidirecional.    |
| **Persistência em JSON**  | Armazenamento local de usuários em arquivo simples.  |
| **Integração front-back** | Comunicação entre formulários HTML e servidor Flask. |


