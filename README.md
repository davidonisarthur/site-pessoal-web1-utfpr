# Site pessoal — Mobile First

- **Aluno:** Arthur Otavio Rodrigues Davidonis.
- **Objetivo:** separar conteúdo HTML e apresentação CSS, com layout Mobile First usando Grid e Flexbox, sem frameworks ou JavaScript na página.
- **Site publicado:** [Acessar o site pessoal](https://davidonisarthur.github.io/site-pessoal-web1-utfpr/).

Abra `index.html` no navegador ou execute `python -m http.server 8000` e acesse http://localhost:8000.

## Layout

O CSS base organiza cabeçalho, menu e seções em uma coluna para celulares. A partir de `48rem` (768 px com fonte padrão), o menu usa uma linha flexível com quebra e as seções passam a duas colunas. A partir de `75rem` (1200 px), os espaçamentos aumentam. As imagens têm `max-width: 100%` e altura automática; os campos ocupam a largura disponível. O formulário é demonstrativo e não envia dados.

## Verificação

Página verificada no Chromium com viewport emulado nas três larguras. Em todas, a imagem carregou, não houve rolagem horizontal e os links de navegação e controles do formulário ficaram dentro da largura disponível.

| Tela | Largura | Evidência |
| --- | --- | --- |
| Mobile | 375 px | [Captura](evidencias/mobile-375.png) |
| Tablet | 768 px | [Captura](evidencias/tablet-768.png) |
| Desktop | 1200 px | [Captura](evidencias/desktop-1200.png) |

As capturas mostram a área inicial de cada viewport. As medições da página estão em [verificacao.json](evidencias/verificacao.json).

Para repetir manualmente, abra o DevTools, ative a barra de dispositivos e configure cada largura. Percorra a página, clique no menu e confira o preenchimento e a limpeza do formulário e o foco ao navegar com Tab.
