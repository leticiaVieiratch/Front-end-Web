# Frontend Web - Consulta de Data e Hora

Interface web limpa e responsiva que consome a API backend de data e hora e exibe os resultados em tempo real na tela.

---

## 🛠️ Tecnologias

- **HTML5**: Estrutura semântica
- **CSS3**: Estilização moderna com gradientes e flexbox
- **JavaScript (ES6+)**: Consumo assíncrono via `fetch`

---

## 🚀 Como Executar Localmente

1. Certifique-se de que a API backend está em execução (`http://localhost:3000`).
2. Abra o arquivo `index.html` diretamente em seu navegador, ou utilize uma extensão de servidor local como o **Live Server** no VS Code.

---

## ⚙️ Configuração da URL da API

No arquivo `index.html`, a URL padrão para desenvolvimento local é:

```javascript
const API_URL = 'http://localhost:3000/data-hora';
```

Quando o backend estiver publicado na nuvem (por exemplo, no Render), atualize essa constante com a URL pública:

```javascript
const API_URL = 'https://SEU-BACKEND.onrender.com/data-hora';
```

---

## ☁️ Deploy

Você pode publicar este frontend gratuitamente em plataformas estáticas como:
- [Vercel](https://vercel.com/)
- [Netlify](https://www.netlify.com/)
- [GitHub Pages](https://pages.github.com/)
