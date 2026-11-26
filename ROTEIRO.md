# Hobby Hub: roteiro de estudos

Site pessoal pra estudar desenvolvimento web, montado **pedaço por pedaço**.
Tema: meus livros, séries e jogos.

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
- [x] Git iniciado e projeto no GitHub (o push eu faço manualmente)

### Como estamos trabalhando
- **Eu escrevo a lógica** (as tags). O Claude **revisa e dá dicas**, sem entregar a resposta pronta.
- **O Claude escreve os comentários didáticos** depois que a estrutura estiver certa.
- **O Claude cuida do recuo (indentação)** do arquivo. Eu foco na lógica.

### Lições que aprendi
- **Toda tag que abre, fecha** (exceções: `<meta>`, `<img>`, `<br>`...). O navegador "conserta" sozinho, mas isso vira bug no CSS.
- **O que é da seção fica no `<section>`; o que é do item fica no `<article>`.** Pergunta-chave: "isso fala deste jogo ou da seção inteira?"
- **Bloco × em linha:** `<p>`, `<h1>`, `<section>` ocupam a linha inteira. `<a>`, `<small>`, `<strong>`, `<em>` ficam lado a lado.
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

---

## Próximos passos (fase HTML)

- [ ] **Jogos:** adicionar um 2º jogo, e talvez um "top 3" com `<ol>` (lista numerada)
- [ ] **Imagens**: capas com `<img>` (atributos `src` e `alt`) e talvez `<figure>` / `<figcaption>`
- [ ] Trocar todo conteúdo `TROQUE` pelo meu conteúdo real
- [ ] (Opcional) Uma seção "Sobre mim" ou um formulário simples (`<form>`, `<input>`, `<label>`)
- [ ] Revisar: decidir se Livros também usa `<dl>` como as Séries, pra padronizar

## Fases depois do HTML
1. **CSS**: aqui entra a personalização do meu jeito (cores, fontes, layout)
2. **Responsividade**: o site ficar bom no celular
3. **JavaScript** (talvez): filtros, contador etc.

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
> "Leia o ROTEIRO.md e vamos continuar do próximo passo, seguindo as regras de lá."
