# Hobby Hub: roteiro de estudos

Site pessoal pra estudar desenvolvimento web, montado **pedaço por pedaço**.
Tema: meus livros, séries, filmes e jogos.

---

## 📍 ONDE PARAMOS (leia isto primeiro)

**Última sessão:** 26/11/2026. **A fase HTML base está concluída.**
**Próximo passo:** começar o **CSS**.

### Como começar o CSS
1. Criar o arquivo `style.css` na mesma pasta do `index.html`.
2. Ligar o CSS ao HTML com uma tag `<link>` dentro do `<head>`. Ela é a tag nova do primeiro passo; pesquise o formato dela ou peça a dica pro Claude.
3. Testar se a ligação funcionou com uma regra bem simples (ex: mudar a cor do fundo) e abrir o `index.html` no navegador.
4. Só depois disso começar a personalização de verdade.

### Antes de estilizar, decidir a cara do site (é DO MEU JEITO)
- [ ] **Clima:** que sensação o site passa? (estante de livros aconchegante, retrô de videogame, cinema escuro, caderno minimalista...)
- [ ] **Referências:** sites, apps, capas de disco ou jogos cujo visual eu curto
- [ ] **Cores:** uma cor que eu amo, uma que não quero de jeito nenhum, fundo claro ou escuro
- [ ] **Letra:** com serifa (mais "livro") ou sem serifa (mais "moderna")

> Evitar a "cara de IA": nada de gradiente roxo/azul genérico, cards todos iguais com sombra suave, emojis decorando tudo. Toda escolha visual tem que ter um motivo meu.

---

## Regras do projeto

1. **Um pedaço por vez.** Cada passo adiciona UMA coisa nova (uma seção, uma tag nova). Nada de fazer tudo de uma vez.
2. **Só HTML por enquanto.** CSS e JavaScript só entram quando eu decidir passar pra próxima fase.
3. **Código todo comentado, didático, em português.** Cada tag nova vem com um comentário explicando o que é, pra que serve e quando usar.
4. **Sem cara de IA.** Nada de layout genérico, gradiente roxo, emoji por todo lado e textos de marketing. A personalização visual é **do meu jeito**: eu decido cores, fontes e estilo na fase do CSS.
5. **Conteúdo de exemplo é provisório.** Onde tiver `TROQUE`, eu coloco meu conteúdo de verdade.
6. **Commits só no meu nome.** Sem linha de coautoria do Claude (`Co-Authored-By`) nem "Generated with Claude".
7. **Salvar sempre.** Commit + push no fim de cada passo, pra nunca mais perder trabalho.

---

## O que já foi feito

### Sessão 1 (26/11/2026)
- [x] Estrutura base: `<!DOCTYPE>`, `<html lang>`, `<head>` (charset, viewport, title), `<body>`
- [x] `<header>` com `<h1>` e subtítulo
- [x] `<nav>` com menu (`<ul>`, `<li>`, `<a href="#...">`)
- [x] `<main>` e `<footer>` (footer ainda vazio)
- [x] Seção **Livros**: `<section id>`, `<h2>`, `<h3>`, `<article>`, `<strong>`, `<em>`
- [x] Seção **Séries**: lista de descrição `<dl>`, `<dt>`, `<dd>` (ficha técnica)
- [x] Seção **Jogos** (feita por mim, revisada): aprendi que toda tag que abre, fecha, e que o título da seção fica FORA do `<article>`
- [x] **Rodapé** (feito por mim, revisado): `<small>`, `&copy;`, link "voltar ao topo" (`id="topo"` no `<h1>`), link externo com `target="_blank"`
- [x] **Seção Filmes** (feita por mim, de primeira!): link no menu + `id`, mesmo molde das outras seções
- [x] `<meta name="description">` no `<head>` + subtítulo atualizado com filmes
- [x] **Livros padronizados com `<dl>`** (feito por mim, revisado): título no `<h3>` dentro do `<article>`, um par `<dt>`+`<dd>` por informação; campos novos Resumo e Páginas
- [x] Git iniciado e projeto no GitHub (o push eu faço manualmente)
- [x] **✅ FASE HTML BASE CONCLUÍDA**

### Como estamos trabalhando
- **Eu escrevo a lógica** (as tags). O Claude **revisa e dá dicas**, sem entregar a resposta pronta.
- **O Claude escreve os comentários didáticos** depois que a estrutura estiver certa.
- **O Claude cuida do recuo (indentação)** do arquivo. Eu foco na lógica.

### Lições que aprendi
- **Toda tag que abre, fecha** (exceções: `<meta>`, `<img>`, `<br>`...). O navegador "conserta" sozinho, mas isso vira bug no CSS.
- **O que é da seção fica no `<section>`; o que é do item fica no `<article>`.** Pergunta-chave: "isso fala deste jogo ou da seção inteira?"
- **Bloco × em linha:** `<p>`, `<h1>`, `<section>` ocupam a linha inteira. `<a>`, `<small>`, `<strong>`, `<em>` ficam lado a lado.
- **`<dl>`: uma informação = um par `<dt>` + `<dd>`.** O `<dt>` é o NOME do campo (Autor, Ano), nunca o conteúdo. O título do item fica no `<h3>`, fora da `<dl>` e dentro do `<article>`.
- **Indentação:** cada nível "dentro" ganha 2 espaços. Não muda nada no navegador, mas mostra quem está dentro de quem.

### Tags que já aprendi
| Tag | Pra que serve |
|---|---|
| `<header>` | Cabeçalho do site (topo) |
| `<nav>` | Bloco de navegação/menu |
| `<main>` | Conteúdo principal (só um por página) |
| `<section>` | Bloco temático, tipo um "capítulo" |
| `<article>` | Conteúdo que faz sentido sozinho (cada livro/série/jogo) |
| `<footer>` | Rodapé |
| `<h1>` a `<h3>` | Títulos em hierarquia: não pular níveis |
| `<p>` | Parágrafo |
| `<ul>` / `<li>` | Lista sem numeração / item da lista |
| `<a href="#id">` | Link que pula pra uma seção da página |
| `<strong>` / `<em>` | Importância (negrito) / ênfase (itálico) |
| `<dl>` / `<dt>` / `<dd>` | Lista de descrição: rótulo → valor |
| `<small>` | "Letras miúdas": créditos, direitos autorais |
| `&copy;` | Entidade HTML que vira © (também `&amp;`, `&lt;`, `&gt;`) |
| `<a href="https://..." target="_blank">` | Link externo que abre em aba nova |
| `<meta name="description">` | Resumo do site pro Google e pra prévias de link (não aparece na página) |

---

## Pendências de HTML (dá pra fazer a qualquer momento)

- [ ] **Jogos:** adicionar um 2º jogo, e talvez um "top 3" com `<ol>` (lista numerada)
- [ ] Trocar todo conteúdo `TROQUE` pelo meu conteúdo real
- [ ] (Opcional) Uma seção "Sobre mim"
- [ ] Formulário de "Adicionar" (`<form>`, `<input>`, `<button>`): fazer junto com a fase do JavaScript
- [ ] Hábito: validar o HTML em validator.w3.org antes de cada fase nova

> **Imagens/capas: NÃO fazer à mão.** Elas vão vir automaticamente da API (ver fase 4).

## Fases depois do HTML
1. **CSS**: aqui entra a personalização do meu jeito (cores, fontes, layout)
2. **Responsividade**: o site ficar bom no celular
3. **JavaScript básico**: filtros, contador etc.
4. **Dados automáticos via API**: cada filme/série/livro/jogo terá um **id**, e o JavaScript vai usar esse id pra puxar de sites externos a capa, a sinopse, o ano, o gênero etc.
   - Filmes/séries: TMDB ou OMDb (o IMDb em si não tem API gratuita aberta)
   - Livros: Open Library ou Google Books
   - Jogos: RAWG ou IGDB
   - **Por que o HTML de agora importa:** os `<article>` com `<dl>` que estou montando viram o "molde" que o JavaScript vai preencher. Então vale pensar desde já em quais campos eu quero (gênero, ano, plataforma...) e o que vai ser meu (status, opinião) e o que vem da API.

---

## Como continuar de outro computador

**Primeira vez no computador novo** (baixa o projeto):
```bash
git clone https://github.com/fabiogomes95/hobby-hub.git
cd hobby-hub
```

**Toda vez antes de começar** (pega o que foi feito no outro PC):
```bash
git pull
```

**Toda vez que terminar um passo** (salva e manda pro GitHub):
```bash
git add .
git commit -m "Descreve aqui o que foi feito"
git push
```

**Pra ver o site:** é só abrir o `index.html` com dois cliques (abre no navegador).

### Se for usar o Claude de novo
Abra a pasta do projeto e diga algo como:
> "Leia o ROTEIRO.md inteiro, principalmente 'Onde paramos', 'Regras do projeto' e 'Como estamos trabalhando'. Vamos continuar do próximo passo (começar o CSS) seguindo essas regras: eu escrevo o código, você revisa com dicas sem me dar a resposta pronta, e depois escreve os comentários didáticos e arruma o recuo. Commits sem coautoria do Claude."

**No fim de cada sessão:** pedir pro Claude atualizar a parte "📍 ONDE PARAMOS" e o "O que já foi feito".
