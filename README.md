# Rotinas de quem? Inspeção semiótica das Rotinas da Alexa

Artigo em desenvolvimento sobre a metacomunicação do aplicativo Amazon Alexa na criação e no gerenciamento de rotinas, considerando a casa como usuário coletivo. O estudo aplica o Método de Inspeção Semiótica (MIS) com uma lente para múltiplos interlocutores e triangula os achados com avaliações públicas do aplicativo.

O texto segue o template Springer LNCS/LNAI (`llncs` v2.26, estilo `splncs04`), usado pelo BRACIS.

## Estrutura

```
.
├── main.tex                  # documento principal e configurações
├── references.bib            # referências (BibTeX), conferidas em fonte primária
├── sections/
│   ├── 00-resumo.tex
│   ├── 01-introducao.tex
│   ├── 02-fundamentacao.tex
│   ├── 03-trabalhos-relacionados.tex
│   ├── 04-metodo.tex
│   ├── 05-resultados.tex
│   ├── 06-discussao.tex
│   ├── 07-limitacoes.tex
│   └── 08-conclusao.tex
├── figures/                  # imagens (prints do app, diagramas)
├── llncs.cls                 # classe oficial Springer LNCS
└── splncs04.bst              # estilo oficial de referências Springer
```

## Como compilar

Localmente, com uma distribuição LaTeX (MiKTeX ou TeX Live):

```
latexmk -pdf main.tex
```

Ou sem `latexmk`: `pdflatex main`, `bibtex main`, `pdflatex main`, `pdflatex main`.

No Overleaf: crie um projeto, envie todos os arquivos (ou importe este repositório pelo GitHub) e compile `main.tex`.

## Chaves de configuração em `main.tex`

| Chave | Uso |
|---|---|
| `\anonymoustrue` / `\anonymousfalse` | O BRACIS usa revisão duplo-anônima. Mantenha `\anonymoustrue` na submissão. |
| `\pendentestrue` / `\pendentesfalse` | Mostra ou esconde as marcações `\pendente{...}` em vermelho. |
| `babel` | O texto está em português. O BRACIS exige inglês: na versão final, troque para `\usepackage[brazilian,english]{babel}`. |

## Requisitos do BRACIS (edição 2026)

- Artigo em inglês, com no máximo 15 páginas, incluindo figuras, tabelas, referências e apêndices.
- Template Springer LNCS, publicado na série LNAI.
- Revisão duplo-anônima: nenhuma informação que identifique autores ou instituições.
- O uso de IA generativa na escrita deve ser declarado nos agradecimentos.

Fonte: [chamada do BRACIS 2026](https://bracis.sbc.org.br/2026/bracis/).

## Licença

O texto do artigo é de autoria dos responsáveis por este repositório. Os arquivos `llncs.cls` e `splncs04.bst` são distribuídos pela Springer Nature sob a licença CC BY 4.0.
