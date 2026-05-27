# 📺 IPTV PRO — Web Player

Player IPTV 100% no navegador, sem backend, sem servidor de vídeo próprio.  
Lê listas **M3U / M3U8** de qualquer provedor IPTV.

## 🚀 Como usar no GitHub Pages

### 1. Criar o repositório
1. Acesse [github.com/new](https://github.com/new)
2. Nome: `iptv-player` (ou qualquer nome)
3. Marque **Public**
4. Clique **Create repository**

### 2. Subir o arquivo
```bash
# Clone o repo
git clone https://github.com/SEU_USUARIO/iptv-player.git
cd iptv-player

# Copie o index.html para esta pasta
# Depois:
git add index.html
git commit -m "feat: add IPTV web player"
git push origin main
```

### 3. Ativar GitHub Pages
1. No repositório → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** / pasta: **/ (root)**
4. Clique **Save**
5. Em ~1 minuto o player estará em:  
   `https://SEU_USUARIO.github.io/iptv-player`

---

## 🎮 Funcionalidades

- ✅ Leitura de listas M3U / M3U8
- ✅ Importação por URL, arquivo ou texto colado
- ✅ Reprodução de streams HLS (via hls.js)
- ✅ Canais favoritos (salvo no navegador)
- ✅ Histórico de canais recentes
- ✅ Busca e filtro por nome/categoria
- ✅ Controles: play/pause, volume, mudo, anterior/próximo
- ✅ Tela cheia
- ✅ Atalhos de teclado

## ⌨️ Atalhos de teclado

| Tecla | Ação |
|-------|------|
| `Espaço` | Play / Pause |
| `→` | Próximo canal |
| `←` | Canal anterior |
| `M` | Mudo |
| `F` | Tela cheia |

## ⚠️ Observações

- O player **não hospeda vídeo** — ele apenas reproduz streams de provedores IPTV.
- Alguns provedores bloqueiam CORS. Nesses casos, use a lista colada diretamente no campo M3U.
- Para URLs M3U, é usado um proxy público (allorigins.win) para contornar CORS.

## 🛠️ Stack

- HTML5 + CSS3 + JavaScript puro (zero dependências locais)
- [hls.js](https://github.com/video-dev/hls.js/) carregado via CDN para streams HLS
- Fontes: Google Fonts (Oxanium + Share Tech Mono)

## 📦 Próximos passos

- [ ] Versão desktop com Electron
- [ ] APK Android com Capacitor
- [ ] Versão Android TV
- [ ] EPG (guia de programação)
- [ ] Suporte a Xtream Codes API
