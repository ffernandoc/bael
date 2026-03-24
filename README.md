# Dragonborn

Site estatico focado em uma experiencia editorial e cinematica para os cinco grandes dragoes.

## Estrutura

- `index.html`: estrutura da pagina
- `styles.css`: layout, tipografia, estados e animacoes
- `script.js`: troca de capitulos, efeitos e renderizacao do painel
- `assets/`: imagens dos dragoes e dos fundos

## Preview local

No diretorio do projeto:

```bash
python3 -m http.server 4173
```

Abra:

```text
http://127.0.0.1:4173
```

## Verificacao rapida

```bash
node --check script.js
```

## Preparar para Git

Se quiser iniciar um repositorio aqui:

```bash
git init
git add .
git commit -m "Polish final do frontend"
```

Depois conecte o remoto normalmente:

```bash
git remote add origin <URL_DO_REPOSITORIO>
git branch -M main
git push -u origin main
```

## Deploy no Cloudflare Pages

Este projeto e totalmente estatico. No Cloudflare Pages, use:

- Framework preset: `None`
- Build command: deixar vazio
- Build output directory: `.`

### Deploy por Git

1. Crie um projeto no Cloudflare Pages.
2. Conecte o repositorio.
3. Use as configuracoes acima.
4. Faça o deploy.

### Deploy por CLI

Com `wrangler`:

```bash
npx wrangler pages deploy .
```

O arquivo `wrangler.toml` ja deixa o diretorio atual como saida do deploy.
