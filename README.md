# Rotinas de quem? Inspeção semiótica das Rotinas da Alexa

Artigo em desenvolvimento sobre a metacomunicação do aplicativo Amazon Alexa e do Echo sobre as rotinas, do ponto de vista de quem as opera e de quem convive com elas. O estudo de caso aplica o Método de Inspeção Semiótica (MIS) guiado por duas personas da mesma casa, fundamentadas na literatura: quem administra a conta e quem convive com as rotinas sem administrá-las.

**PDF mais recente:** [main.pdf](main.pdf)

O texto segue o **template acessível de uma coluna da SBC**, exigido nas trilhas de artigos completos do IHC 2026 (XXV Simpósio Brasileiro sobre Fatores Humanos em Sistemas Computacionais, Quixadá/CE).

## Estrutura

```
.
├── main.tex                       # documento principal e configurações
├── main.pdf                       # versão compilada mais recente
├── references.bib                 # referências (BibTeX), conferidas em fonte primária
├── IHC_info.tex                   # trilha, local, ano e edição do evento (cabeçalho)
├── sections/
│   ├── 00-resumo.tex              # Abstract e Resumo estruturados
│   ├── 01-introducao.tex
│   ├── 02-fundamentacao.tex       # inclui os trabalhos relacionados
│   ├── 03-metodo.tex
│   ├── 04-resultados.tex
│   ├── 05-discussao.tex
│   ├── 06-limitacoes.tex
│   ├── 07-conclusao.tex
│   ├── 08-consideracoes-eticas.tex
│   └── 09-agradecimentos.tex
├── figures/                       # imagens (prints do app, diagramas)
├── sbc-template.sty               # estilo oficial SBC (margens, fontes, títulos)
├── IHC.sty                        # cabeçalho do IHC
└── sbc.bst                        # estilo oficial de referências SBC (autor-ano)
```

## Como compilar

Localmente, com uma distribuição LaTeX (MiKTeX ou TeX Live):

```
latexmk -pdf main.tex
```

Ou sem `latexmk`: `pdflatex main`, `bibtex main`, `pdflatex main`, `pdflatex main`.

No Overleaf: *New Project → Import from GitHub*, selecione este repositório e compile `main.tex`.

Os trechos ainda não escritos aparecem em vermelho como `[PENDENTE: ...]`. Para gerar uma versão sem eles, troque `\pendentestrue` por `\pendentesfalse` em `main.tex`.

## Formato exigido pelo IHC 2026

- Folha A4, uma coluna; margens de 3,5 cm (superior), 2,5 cm (inferior) e 3 cm (laterais).
- Times 12 pt, títulos de seção em 13 pt e título do artigo em 16 pt, em negrito.
- Resumo estruturado (Introdução, Objetivo, Metodologia, Resultados), com no máximo 10 linhas; em artigos em português, Abstract e Resumo são obrigatórios.
- Sugestão de 15 a 20 páginas, sem contar as referências. O texto pode ser em português ou inglês.
- Seção obrigatória "Considerações Éticas", com base nas Resoluções CNS n.º 466/2012, 510/2016 e 674/2022, e medidas de proteção de dados conforme a LGPD.
- Declaração do uso de IA generativa na escrita, de preferência nos Agradecimentos.
- Figuras com descrição acessível via `\pdftooltip{...}{descrição}` (pacote `pdfcomment`).

Fonte: [instruções para artigos completos do IHC 2026](https://ihc.sbc.org.br/2026/index.php/en/full-papers/).

## Licença

O texto do artigo é de autoria dos responsáveis por este repositório. Os arquivos de estilo (`sbc-template.sty`, `IHC.sty`, `sbc.bst`) são do template oficial da SBC e do IHC 2026.
