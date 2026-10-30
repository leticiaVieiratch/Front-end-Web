# 🌐 Front-end Web: Consulta de Data e Hora

[![Node.js](https://img.shields.io/badge/Node.js-v18+-green?logo=node.js)](https://nodejs.org/)
[![Express](https://img.shields.io/badge/Express-v4.19-lightgrey?logo=express)](https://expressjs.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow?logo=javascript)](https://developer.mozilla.org/)
[![HTML5](https://img.shields.io/badge/HTML5-Semântico-orange?logo=html5)](https://developer.mozilla.org/)
[![CSS3](https://img.shields.io/badge/CSS3-Moderno-blue?logo=css3)](https://developer.mozilla.org/)

Aplicação **Full Stack** completa que integra um **Frontend Web moderno e responsivo** a uma **API Backend em Node.js/Express** para consulta e exibição da data e hora do servidor em tempo real.

---

## 📁 Estrutura do Projeto

O repositório é organizado de forma modular, separando a camada de interface (frontend) e a camada de serviços (backend):

```text
Front-end-Web/
├── api-back/             # Camada de Backend (API REST)
│   ├── .gitignore        # Arquivos ignorados pelo Git (node_modules, etc.)
│   ├── api.js            # Código principal do servidor Express
│   ├── package.json      # Metadados e dependências do Node.js
│   └── README.md         # Documentação específica da API
│
├── api-front/            # Camada de Frontend (Interface Web)
│   ├── index.html        # Estrutura HTML e lógica de consumo da API via fetch
│   ├── style.css         # Estilização visual moderna e responsiva
│   └── README.md         # Documentação específica da interface
│
├── .gitignore            # Ignora pastas de dependências globais
└── README.md             # Documentação geral do repositório
```

---

## 🛠️ Tecnologias Utilizadas

### **Backend (`api-back`)**
- **Node.js**: Ambiente de execução JavaScript no servidor.
- **Express**: Framework web minimalista para criação de rotas REST.
- **CORS**: Middleware para permitir requisições de origens cruzadas pelo navegador.

### **Frontend (`api-front`)**
- **HTML5**: Estrutura semântica e acessível.
- **CSS3**: Layout moderno centralizado com gradientes, sombras e responsividade.
- **JavaScript Vanilla (ES6+)**: Consumo assíncrono de API via `fetch` e manipulação dinâmica do DOM.

---

## 🚀 Como Executar o Projeto Localmente

### 1. Pré-requisitos
- [Node.js](https://nodejs.org/) versão 18 ou superior instalado.
- [Git](https://git-scm.com/) instalado.

### 2. Clonar o Repositório
```bash
git clone https://github.com/leticiaVieiratch/Front-end-Web.git
cd Front-end-Web
```

---

### 3. Rodando o Backend (`api-back`)

1. Entre na pasta do backend:
   ```bash
   cd api-back
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. Inicie o servidor:
   ```bash
   npm start
   ```

4. O servidor estará ativo em:
   ```
   http://localhost:3000
   ```

---

### 4. Rodando o Frontend (`api-front`)

1. Abra uma nova aba de terminal ou utilize o explorador de arquivos.
2. Navegue até a pasta `api-front`:
   ```bash
   cd api-front
   ```
3. Abra o arquivo `index.html` em qualquer navegador (dê um duplo clique ou use a extensão **Live Server** do VS Code).
4. O frontend irá carregar automaticamente a data e hora do servidor local e disponibilizar o botão **Atualizar** para novas consultas.

---

## 🔌 Documentação da API

| Método | Rota | Descrição |
|---|---|---|
| `GET` | `/` | Rota raiz de teste de funcionamento da API |
| `GET` | `/data-hora` | Retorna a data e hora atual do servidor |

### Exemplo de Resposta (`GET /data-hora`):
```json
{
  "dataHoraCompleta": "2026-10-29T01:30:57.874Z",
  "data": "28/10/2026",
  "hora": "22:30:57",
  "timestamp": 1793237457874
}
```

---

## 🌐 Guia de Deploy

### **Deploy do Backend (ex: Render)**
1. Acesse [render.com](https://render.com) e crie um **Web Service**.
2. Aponte para este repositório no GitHub.
3. Defina:
   - **Root Directory**: `api-back`
   - **Build Command**: `npm install`
   - **Start Command**: `npm start`
4. Copie a URL pública gerada (ex: `https://seu-backend.onrender.com`).

### **Deploy do Frontend (ex: Vercel / Netlify / GitHub Pages)**
1. No arquivo `api-front/index.html`, atualize a constante `API_URL` com a URL pública do seu backend:
   ```javascript
   const API_URL = 'https://seu-backend.onrender.com/data-hora';
   ```
2. Faça o deploy da pasta `api-front` na plataforma escolhida.

---

## 👩‍💻 Autora

Desenvolvido por **[Letícia Vieira](https://github.com/leticiaVieiratch)**.
