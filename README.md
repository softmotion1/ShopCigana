# 🛒 ShopCigana — Discord Shop

> Loja de produtos digitais integrada com Discord. Simples, rápida e sem necessidade de backend.

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)

---

## 📸 Preview

<div align="center">

| Loja | Carrinho | Checkout |
|------|----------|----------|
| Grelha de produtos com filtros e pesquisa | Sidebar lateral com resumo | Formulário em 3 passos |

</div>

---

## ✨ Funcionalidades

- **115+ produtos** organizados em 11 categorias
- **Filtros por categoria** + barra de pesquisa em tempo real
- **Carrinho lateral** com produtos, quantidades e total
- **Checkout em 3 passos** — dados pessoais → pagamento → confirmação
- **4 métodos de pagamento** — Crypto, PayPal, MBWay e Referência MB/ATM
- **Integração com Discord** — pedido finalizado via ticket no servidor
- **100% client-side** — sem backend, sem base de dados, sem servidor
- **Design responsivo** — funciona em mobile e desktop
- **Tema azul/roxo** inspirado no Discord

---

## 🗂️ Categorias de Produtos

| Categoria | Exemplos |
|-----------|---------|
| 💬 Discord | Contas verificadas, Nitro, Boosts, Generator |
| 🎯 Fortnite | Skins OG, V-Bucks, Contas ranked |
| 🔫 CS2 | Contas Prime, NFA, Hours |
| ⚔️ Valorant | Contas EU com skins e Knife |
| 🦾 Apex Legends | Contas ranked por nível |
| 🧱 Roblox | Robux (1k a 50k) |
| 🛡️ Spoofers | FiveM, All Games (temp/perm) |
| 🎬 Streaming | Netflix, Spotify, Disney+, HBO Max, Prime Video |
| 🔒 VPN | NordVPN, CyberGhost, TunnelBear, HotSpot Shield |
| 📱 Social | Instagram, TikTok, Twitch, YouTube followers |
| 👤 Contas | Minecraft, GTA 5, Rust, Black Ops, Clash Royale, Valorant... |
| 🔧 Tools | Rockstar Tool, Lusive Software, Generators, Methods |

---

## 💳 Métodos de Pagamento

| Método | Descrição |
|--------|-----------|
| ₿ **Crypto** | Bitcoin (BTC), Ethereum (ETH), USDT TRC20/ERC20 |
| 🅿 **PayPal** | Apenas "Amigos e Família" para evitar taxas |
| 📱 **MBWay** | Transferência instantânea pelo app MB WAY |
| 🏧 **Código MB** | Referência Multibanco / Código de Levantamento ATM |

> Todos os pagamentos são processados via **ticket no Discord** após confirmação do pedido.

---

## 🚀 Como Usar

### 1. Clonar o repositório

```bash
git clone https://github.com/teu-user/shopcigana.git
cd shopcigana
```

### 2. Abrir o ficheiro

Basta abrir o `shopcigana.html` num browser — não é necessário nenhum servidor.

```bash
# Opcionalmente, servir com um servidor local
npx serve .
# ou
python3 -m http.server 8080
```

### 3. Configurar o link do Discord

Dentro do ficheiro `shopcigana.html`, encontra o botão de ticket e substitui o `href` pelo link do teu servidor Discord:

```html
<a href="https://discord.gg/SEU-LINK" class="btn-discord">
  💬 Abrir Ticket no Discord
</a>
```

---

## ⚙️ Personalização

### Alterar o nome da loja

```html
<!-- Linha ~235 no ficheiro HTML -->
<div class="logo">Shop<span>Cigana</span></div>
```

### Adicionar/editar produtos

Os produtos estão definidos no array `PRODS` no JavaScript:

```javascript
{
  id: 999,           // ID único
  n: 'Nome do Produto',
  c: 'Categoria',    // Discord, Fortnite, CS2, etc.
  p: 9.99,           // Preço em euros
  s: 50,             // Stock disponível (0 = esgotado)
  b: 'Hot',          // Badge opcional: 'Hot', 'Novo', 'Raro', 'Popular'
  bt: 'hot'          // Tipo do badge (para cor): 'hot' | 'new' | omitir para roxo
}
```

### Alterar preços em massa

Para aumentar todos os preços em X%, edita o array com um script ou usa find & replace com regex.

---

## 📁 Estrutura

```
shopcigana/
│
├── shopcigana.html    # Ficheiro único — loja completa (HTML + CSS + JS)
└── README.md          # Este ficheiro
```

> Toda a loja está contida num **único ficheiro HTML** — fácil de hospedar em qualquer lugar.

---

## 🌐 Hospedagem Gratuita

Podes hospedar o site gratuitamente em várias plataformas:

| Plataforma | Como |
|------------|------|
| **GitHub Pages** | Faz push do ficheiro e ativa em Settings → Pages |
| **Netlify** | Arrasta o ficheiro para [netlify.com/drop](https://app.netlify.com/drop) |
| **Vercel** | `vercel --prod` na pasta do projeto |
| **Cloudflare Pages** | Liga ao repositório GitHub |

---

## 🔄 Fluxo de Compra

```
Cliente visita o site
       ↓
Escolhe produto(s) → Adiciona ao carrinho
       ↓
Clica em "Finalizar compra"
       ↓
Passo 1: Preenche nome, email e username Discord
       ↓
Passo 2: Escolhe método de pagamento
       ↓
Passo 3: Recebe nº de pedido gerado automaticamente
       ↓
Abre ticket no Discord com o nº de pedido
       ↓
Staff envia dados de pagamento e confirma entrega
```

---

## 🛠️ Tecnologias

- **HTML5** + **CSS3** + **JavaScript** vanilla — sem frameworks
- **Google Fonts** — Syne (títulos) + DM Sans (corpo)
- Design inspirado no tema escuro do Discord

---

## 📄 Licença

Este projeto é de uso pessoal. Não redistribuir sem autorização.

---

<div align="center">
  Feito com 💜 para o servidor Discord
</div>
