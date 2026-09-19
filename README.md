# Vektra Projetos — Landing Page

Landing page estática (HTML/CSS/JS puro, sem build) para mostrar exemplos de
projetos da Vektra Projetos e captar contacto via WhatsApp.

## Estrutura

```
vektra-landing/
├── index.html
├── css/style.css
├── js/script.js
├── images/        ← imagens dos projetos (renders 3D)
└── README.md
```

## Publicar no GitHub Pages

1. Cria um repositório novo no GitHub (ex.: `vektra-landing`).
2. Envia estes ficheiros para o repositório, mantendo a mesma estrutura de pastas:
   ```
   git init
   git add .
   git commit -m "Landing page Vektra Projetos"
   git branch -M main
   git remote add origin https://github.com/SEU-UTILIZADOR/vektra-landing.git
   git push -u origin main
   ```
3. No GitHub, vai a **Settings → Pages**.
4. Em **Source**, seleciona a branch `main` e a pasta `/ (root)`.
5. Guarda. Em 1–2 minutos o site fica disponível em:
   `https://SEU-UTILIZADOR.github.io/vektra-landing/`

## Domínio próprio (opcional)

Se quiseres usar um domínio próprio (ex. `vektraprojetos.com`):
1. Cria um ficheiro `CNAME` na raiz do repositório com o domínio dentro.
2. Configura o DNS do domínio a apontar para o GitHub Pages (registo `A` para
   os IPs do GitHub, ou `CNAME` para `SEU-UTILIZADOR.github.io`).
3. Ativa o domínio em **Settings → Pages → Custom domain**.

## Editar conteúdo

- **Textos e projetos**: editar diretamente `index.html` (cada projeto é um
  bloco `<article class="sheet">`).
- **Número de WhatsApp**: procurar por `934225828` em `index.html` (há 2
  ocorrências nos botões de contacto e 1 no link `tel:`).
- **Cores/tipografia**: variáveis no topo de `css/style.css` (`:root { ... }`).

## Notas

- Sem dependências além de duas famílias tipográficas do Google Fonts
  (Big Shoulders Display + IBM Plex).
- Totalmente responsivo, com menu de hambúrguer em ecrãs estreitos.
- As imagens já estão otimizadas o suficiente para web; se quiseres reduzir
  ainda mais o tamanho, podes comprimir os PNGs em `images/` antes do commit.
