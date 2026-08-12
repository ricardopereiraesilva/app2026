# Site de apresentação — Pesquisa Eleitoral 2026

Landing page (site de apresentação) do aplicativo de pesquisa eleitoral.
Público-alvo: potenciais clientes — **ONGs, partidos políticos, empresas e
pessoas físicas**. Apresenta apenas os papéis de **coordenador(a) de pesquisa**
e **entrevistador(a)** (os demais perfis não entram na visão do cliente).

Desenvolvido por **SSSN 7 — Pesquisas Eletrônicas** (o site institucional da empresa
fica em `web_page/empresa/`).

## Tecnologia

HTML + CSS + JS puros, **sem framework e sem build**. Tema escuro ("dark")
moderno, responsivo (mobile-first). Nada de `node_modules`.

## Como visualizar

Abra `index.html` direto no navegador (duplo clique) ou sirva a pasta:

```
# opcional, para servir localmente
python -m http.server 8080   # depois acesse http://localhost:8080
```

## Estrutura

```
web_page/aplicativo/
├── index.html          página única (seções roláveis)
├── css/styles.css      tema, layout e responsividade
├── js/main.js          menu mobile + animações de entrada
├── assets/img/         screenshots do app + favicon.svg
└── README.md           este arquivo
```

As imagens em `assets/img/` são cópias dos screenshots dos guias de usuário
(`user_guide/`) — o site é autocontido e não depende daquela pasta.

> **Recapturas realizadas (2026-07-02):** após a remoção da funcionalidade
> *Metodologia* e a inclusão do item de menu *Instalar aplicativo* (+ novo cartão
> "Entrevistadores da pesquisa"), duas imagens usadas aqui foram substituídas
> pelas versões recapturadas do guia do coordenador (ver
> `user_guide/coordenador/images/CAPTURAS.md`): **`coord-boasvindas.png`** (=
> guia `07-boas-vindas.png`, menu com *Instalar aplicativo*) e **`coord-painel.png`**
> (= guia `08-painel-gestao.png`, com o cartão de entrevistadores). Nenhuma
> alteração de texto na página foi necessária — as menções a "metodologia" são o
> conceito de marketing ("sua pesquisa, sua metodologia"), não a funcionalidade.

## Links (já publicados)

Os destinos já apontam para o que está no ar (abrem em nova aba):

- **Aplicativo (mock)** — https://ricardopereiraesilva.github.io/pe2026
- **Manual do coordenador** — https://ricardopereiraesilva.github.io/coordenador/
- **Manual do entrevistador** — https://ricardopereiraesilva.github.io/entrevistador/

O link do aplicativo aparece na navbar, no hero e no CTA final. Os links dos
manuais aparecem só na seção de papéis (coordenador/entrevistador) e no CTA/rodapé.

## Pendências

> ### ⏸️ Pendências ADIADAS (2026-08-07)
>
> Depois de interação com o Roberto Silvino, as pendências desta pasta ficam **adiadas**:
> serão tratadas **por ele**, na versão que vai publicar — inclusive as do aplicativo —,
> com a **substituição das URLs dos links** para os endereços definitivos.
>
> **Quando retomarmos, o primeiro passo é analisar o que estiver publicado por ele** —
> não reabrir esta lista às cegas. Boa parte do que está abaixo pode ter deixado de
> existir, e o que sobrar terá de ser reescrito contra as URLs novas.

- **"Abrir o aplicativo" leva ao protótipo.** Os links do topo, do corpo, da
  chamada final e do rodapé apontam para `pe2026`, que é o mock publicado — sem
  backend e sem persistência —, enquanto o texto ao lado promete "comece pelo modo
  de avaliação, sem compromisso". Quando o ambiente `avaliacao` existir
  ([pe-docs#205](https://github.com/robertosilvino/pe-docs/issues/205)), estes links
  passam a apontar para ele.
- **Termos do coordenador não são públicos.** O consultor já tem os dele publicados
  no site da SSSN 7 (`termos-consultor.html`); os do cliente só existem dentro do
  aplicativo. As fontes canônicas estão em `Docs/`, prontas para gerar a página.
- **Sem política de privacidade** — o site carrega fontes do Google (terceiro).

## Notas

- Primeiro esboço. Conteúdo e imagens podem ser ajustados.
- **Publicado** no repositório público `ricardopereiraesilva/app2026` (GitHub Pages,
  `main`/raiz) → **https://ricardopereiraesilva.github.io/app2026/**. Republicar =
  clonar o `app2026`, copiar os arquivos alterados desta pasta, commitar e
  `git push origin main`. (A nota anterior dizia "sem deploy configurado" — está
  publicado desde 02/07/2026.)
