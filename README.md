# 🌐 Consulta de Data e Hora

Aplicação Full Stack que consome e exibe em tempo real a data e a hora fornecidas por uma API backend.

---

## 🔗 Links da Aplicação

- 🖥️ **Frontend (Vercel):** [Acessar Aplicação](https://apiprojeto-git-main-leticiavieiratchs-projects.vercel.app/)
- ⚙️ **API Backend (Render):** [https://api-back4.onrender.com/data-hora](https://api-back4.onrender.com/data-hora)

---

## 🛠️ Tecnologias

- **Frontend:** HTML5, CSS3, JavaScript (Fetch API)
- **Backend:** Node.js, Express, CORS
- **Deploy:** Vercel & Render

---

## 🚀 Execução Local

```bash
# Backend (porta 3000)
cd api-back
npm install
npm start

# Frontend
# Abrir o arquivo api-front/index.html no navegador
```

---

## 🔌 Endpoints

- `GET /` — Status da API
- `GET /data-hora` — Retorna a data e hora atual do servidor

```json
{
  "data": "30/10/2026",
  "hora": "20:00:00",
  "dataHoraCompleta": "2026-10-30T23:00:00.000Z",
  "timestamp": 1793410800000
}
```
