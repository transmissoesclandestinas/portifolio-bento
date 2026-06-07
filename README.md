# Portfólio — Bento

Site de portfólio em HTML + CSS + JavaScript puro. Sem build, 100% estático.

## Estrutura
- `index.html` — Home: header + projetos em tela cheia (vídeo/imagem + nome).
- `projeto.html` — Página de projeto (template): título, autores, filtros, mídias e texto.
- `videos/` — onde ficam os arquivos `.webm`/`.webp` das capas (por enquanto).

> O conteúdo está temporariamente escrito dentro de cada HTML (nas listas
> `projetos` e `projeto`). Próximo passo: puxar do Sanity via `fetch`.

## Rodar localmente
Abra o `index.html` no navegador. Para o fluxo de navegação funcionar
(home → projeto → home), abra a partir da pasta inteira.

## Deploy

### 1. GitHub
```bash
cd portfolio-bento
git init
git add .
git commit -m "Primeiro commit — portfolio Bento"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/portfolio-bento.git
git push -u origin main
```

### 2. Vercel
1. vercel.com → New Project → Import Git Repository → selecione o repo.
2. Framework Preset: **Other** (site estático, sem build).
3. Deploy.

Pronto. Cada push novo no GitHub re-publica automático.
