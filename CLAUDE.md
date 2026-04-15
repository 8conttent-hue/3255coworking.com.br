# CLAUDE.md — 3255COWORKING

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** 3255COWORKING
**Nicho:** Negócios e Empreendedorismo
**Keywords:** Ola Me chamo Rogerio Rodrigues sou o criador do website 3255coworking com
**Paleta de cores:** gold | **Fonte:** playfair

Olá! Me chamo Rogério Rodrigues, sou o criador do website 3255coworking.com.br, criei esse portal no intuito de compartilhar minhas experiências que adquiri ao longo dos anos trabalhando na área de coworking. Tenho mais de 10 anos de experiência na gestão e operação de espaços para coworking, sempre buscando inovar e trazer as melhores soluções para meus clientes.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-E |
| Hero | Hero-G |
| Features | Features-D |
| About Section | About-E |
| Posts | Posts-D |
| Footer | Footer-I |
| Página Sobre | Sobre-B |
| Página Contato | Contato-C |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
