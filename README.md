# Site de apresentação — Pesquisa Eleitoral 2026

Landing page (site de apresentação) do aplicativo de pesquisa eleitoral.
Público-alvo: potenciais clientes — **ONGs, partidos políticos, empresas e
pessoas físicas**. Apresenta apenas os papéis de **coordenador(a) de pesquisa**
e **entrevistador(a)** (os demais perfis não entram na visão do cliente).

Desenvolvido por **Floripa E-Pesquisa**.

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
web_page/
├── index.html          página única (seções roláveis)
├── css/styles.css      tema, layout e responsividade
├── js/main.js          menu mobile + animações de entrada
├── assets/img/         screenshots do app + favicon.svg
└── README.md           este arquivo
```

As imagens em `assets/img/` são cópias dos screenshots dos guias de usuário
(`user_guide/`) — o site é autocontido e não depende daquela pasta.

## Links (já publicados)

Os destinos já apontam para o que está no ar (abrem em nova aba):

- **Aplicativo (mock)** — https://ricardopereiraesilva.github.io/pe2026
- **Manual do coordenador** — https://ricardopereiraesilva.github.io/coordenador/
- **Manual do entrevistador** — https://ricardopereiraesilva.github.io/entrevistador/

O link do aplicativo aparece na navbar, no hero e no CTA final. Os links dos
manuais aparecem só na seção de papéis (coordenador/entrevistador) e no CTA/rodapé.

## Notas

- Primeiro esboço. Conteúdo e imagens podem ser ajustados.
- Sem deploy configurado — publicação só quando solicitada.
