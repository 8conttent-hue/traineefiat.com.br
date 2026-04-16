# CLAUDE.md — TRAINEEFIAT

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** TRAINEEFIAT
**Nicho:** Automotivo
**Keywords:** O grupo Fiat A Fiat Automoveis faz parte da Fiat S p
**Paleta de cores:** forest | **Fonte:** playfair

O grupo Fiat A Fiat Automóveis faz parte da Fiat S.p.A, juntamente com outras grande marcas: Lancia, Alfa Romeo, Abarth, Maserati, Ferrari, Chrysler, Jeep, Dodge, SRT, Mopar e… Ram. Fundada Fiat automóveis A fábrica da Fiat Automóveis foi inaugurada em 9 de julho de 1976, em Betim (MG), produzindo o modelo Fiat 147. Está instalada em terreno PASSO A PASSO DA PRODUÇÃO Cada produto Fiat traz consigo a responsabilidade de representar uma das maiores indústrias do país. Uma responsabilidade que está em cada detalhe do que a O PROGRAMA O Programa Trainee Fiat Chysler 2015 tem o objetivo de identificar e desenvolver engenheiros com interesse em atuação na área industrial, que sejam movidos pela paixão e interessados na construção de uma sólida carreira na Fiat Chrysler, unidade de Betim em Minas Gerais ou na unidade de Goiana, no estado de Pernambuco. ETAPAS DE SELEÇÃO A convocação para todas as etapas será realizada por meio do e-mail fornecido pelo candidato no momento da inscrição. Consulte-o sempre e esteja atualizado quanto ao processo seletivo. ETAPA 1 Inscrição 25 de agosto a 29 de setembro ETAPA 2 Testes online ETAPA 3 Check up de competências ETAPA 4 Avaliação de aderência à organização ETAPA 5 Assessment Center e entrevista com os gestores ETAPA 6 Etapas admissionais Importante



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-E |
| Hero | Hero-G |
| Features | Features-H |
| About Section | About-E |
| Posts | Posts-C |
| Footer | Footer-B |
| Página Sobre | Sobre-G |
| Página Contato | Contato-E |

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
