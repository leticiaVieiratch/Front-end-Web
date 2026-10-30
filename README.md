# 🌐 Front-end Web: Consulta de Data e Hora

[![Node.js](https://img.shields.io/badge/Node.js-v18+-green?logo=node.js)](https://nodejs.org/)
[![Express](https://img.shields.io/badge/Express-v4.19-lightgrey?logo=express)](https://expressjs.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow?logo=javascript)](https://developer.mozilla.org/)
[![HTML5](https://img.shields.io/badge/HTML5-Semântico-orange?logo=html5)](https://developer.mozilla.org/)
[![CSS3](https://img.shields.io/badge/CSS3-Moderno-blue?logo=css3)](https://developer.mozilla.org/)
[![Vercel](https://img.shields.io/badge/Deploy-Vercel-black?logo=vercel)](https://apiprojeto-git-main-leticiavieiratchs-projects.vercel.app/)
[![Render](https://img.shields.io/badge/Deploy-Render-46E3B7?logo=render)](https://api-back4.onrender.com)

Aplicação **Full Stack** completa que integra um **Frontend Web moderno e responsivo** a uma **API Backend em Node.js/Express** para consulta e exibição da data e hora do servidor em tempo real.

---

## 🔗 Aplicação no Ar (Produção)

| Componente | Plataforma | Link de Acesso |
|---|---|---|
| 🖥️ **Frontend Web** | Vercel | [https://apiprojeto-git-main-leticiavieiratchs-projects.vercel.app/](https://apiprojeto-git-main-leticiavieiratchs-projects.vercel.app/) |
| ⚙️ **Backend API (Status)** | Render | [https://api-back4.onrender.com](https://api-back4.onrender.com) |
| 🕒 **Endpoint Data e Hora** | Render | [https://api-back4.onrender.com/data-hora](https://api-back4.onrender.com/data-hora) |

---

## 📁 Estrutura do Projeto

O repositório é organizado de forma modular, separando a camada de interface (frontend) e a camada de serviços (backend):

```text
Front-end-Web/
├── api-back/             # Camada de Backend (API REST Node.js/Express)
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
- **Hospedagem**: [Render](https://render.com).

### **Frontend (`api-front`)**
- **HTML5**: Estrutura semântica e acessível.
- **CSS3**: Layout moderno centralizado com gradientes, sombras e responsividade.
- **JavaScript Vanilla (ES6+)**: Consumo assíncrono de API via `fetch` e manipulação dinâmica do DOM.
- **Hospedagem**: [Vercel](https://vercel.com).

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
4. O frontend irá carregar automaticamente a data e hora do servidor e disponibilizar o botão **Atualizar** para novas consultas.

---

## 🔌 Documentação da API

| Método | Rota | Descrição | URL de Produção |
|---|---|---|---|
| `GET` | `/` | Status da API | [https://api-back4.onrender.com](https://api-back4.onrender.com) |
| `GET` | `/data-hora` | Retorna data e hora atual | [https://api-back4.onrender.com/data-hora](https://api-back4.onrender.com/data-hora) |

### Exemplo de Resposta (`GET /data-hora`):
```json
{
  "dataHoraCompleta": "2026-10-30T01:01:17.455Z",
  "data": "29/10/2026",
  "hora": "22:01:17",
  "timestamp": 1793322077455
}
```

---

## 🌐 Deploy em Produção

- **Frontend**: Hospedado na [Vercel](https://apiprojeto-git-main-leticiavieiratchs-projects.vercel.app/) com deploy contínuo integrado ao GitHub.
- **Backend**: Hospedado no [Render](https://api-back4.onrender.com) como Web Service Node.js.

---

## 👩‍💻 Autora

Desenvolvido por **[Letícia Vieira](https://github.com/leticiaVieiratch)**.
