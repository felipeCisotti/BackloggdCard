# Backloggd Card

Gerador de “card” estilo Backloggd (formato 720x1280) direto no navegador.  
Você escolhe o jogo (manual ou via RAWG), coloca fundo/capa/avatar, ajusta tudo no canvas e exporta em PNG.

---

## ✅ O que esse projeto faz

- Cria um card vertical **720x1280** (bom pra Stories/Reels/TikTok)
- Permite:
  - Digitar **título**
  - Escolher **quantidade de estrelas**
  - Inserir imagens por upload: **Fundo**, **Capa do jogo**, **Avatar**
  - Buscar imagens automaticamente pelo **RAWG** (API de jogos)
  - **Arrastar / redimensionar / rotacionar** os elementos no canvas
  - **Exportar** como `.png`

---

## 📦 Como baixar e rodar (bem leigo)

### Opção A) Rodar só com 1 arquivo (mais fácil)
1. Crie uma pasta no seu PC (ex: `backloggd-card`)
2. Dentro dela crie um arquivo chamado:
   - `index.html`
3. Copie e cole **todo o código** do projeto dentro desse `index.html`
4. Salve
5. Clique **duas vezes** no `index.html` pra abrir no navegador (Chrome/Edge/Firefox)

✅ Pronto, já abre o editor.

---

### Opção B) Rodar com servidor local (recomendado pra evitar problemas de imagens/API)
Se você tiver o **VS Code**:

1. Abra o VS Code
2. Instale a extensão: **Live Server**
3. Abra a pasta do projeto
4. Clique com o botão direito em `index.html` → **Open with Live Server**

Isso ajuda principalmente quando você usa imagens externas.

---

## 🔑 Como colocar a KEY da RAWG (pra funcionar o botão “Buscar imagens”)

O projeto usa a API do RAWG pra buscar imagens automaticamente.

### 1) Criar uma conta e pegar a key
1. Vá no site do RAWG (pesquise no Google: **RAWG API key**)
2. Crie uma conta
3. Pegue a sua **API Key** (fica no painel/conta)

> A key é um texto tipo: `123abc456def...`

### 2) Colar a key no código
No seu `index.html`, procure esta linha:

```js
const RAWG_KEY = 'INSIRA SUA KEY AQUI PAIZAO OU PAIZONA (INSERT THE KEY)';

