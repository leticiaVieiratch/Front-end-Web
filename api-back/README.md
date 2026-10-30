# API Backend - Data e Hora

Backend desenvolvido em **Node.js** com **Express** que fornece a data e a hora atual do servidor em formato JSON, com suporte a CORS para consumo por aplicações frontend.

---

## 🔗 API no Ar (Produção)

- **URL Base (Render)**: [https://api-back4.onrender.com](https://api-back4.onrender.com)
- **Endpoint Data/Hora**: [https://api-back4.onrender.com/data-hora](https://api-back4.onrender.com/data-hora)
- **Frontend em Produção (Vercel)**: [https://apiprojeto-git-main-leticiavieiratchs-projects.vercel.app/](https://apiprojeto-git-main-leticiavieiratchs-projects.vercel.app/)

---

## 🛠️ Tecnologias

- [Node.js](https://nodejs.org/) (v18+)
- [Express](https://expressjs.com/)
- [CORS](https://www.npmjs.com/package/cors)

---

## 🚀 Como Executar Localmente

1. Navegue até esta pasta:
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

4. A API estará disponível em:
   ```
   http://localhost:3000
   ```

---

## 🔌 Endpoints

### `GET /`
Verificação de status da API.

- **URL de Produção**: `https://api-back4.onrender.com/`

**Resposta de Exemplo:**
```json
{
  "mensagem": "API de Data e Hora está funcionando!",
  "endpoint": "/data-hora"
}
```

### `GET /data-hora`
Retorna a data e o horário atual no fuso horário `America/Sao_Paulo`.

- **URL de Produção**: `https://api-back4.onrender.com/data-hora`

**Resposta de Exemplo:**
```json
{
  "dataHoraCompleta": "2026-10-30T01:01:17.455Z",
  "data": "29/10/2026",
  "hora": "22:01:17",
  "timestamp": 1793322077455
}
```

---

## ☁️ Deploy no Render

1. Acesse [Render.com](https://render.com) e crie um novo **Web Service**.
2. Conecte este repositório.
3. Configure:
   - **Root Directory**: `api-back`
   - **Build Command**: `npm install`
   - **Start Command**: `npm start`
4. A API estará disponível publicamente na URL configurada.
