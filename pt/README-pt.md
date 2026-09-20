# Protótipo em português — Guerra no Irã

Este diretório contém a **versão em português** do protótipo. É uma matéria jornalística fictícia sobre uma reunião emergencial do Conselho de Segurança da ONU, exibida como se estivesse em um site de notícias real.

## Arquivos

| Arquivo | O que é |
|---|---|
| `index.html` | O protótipo completo — abra em qualquer navegador |

## Como visualizar

Basta abrir `index.html` no navegador. Se o repositório estiver publicado via GitHub Pages, o mesmo conteúdo está disponível em:

```
https://liviasouzavieira.github.io/prototipo-correcao-jornalismo/pt/
```

## O que observar

A matéria fictícia mostra, dentro de um contexto de leitura comum a um site de notícias, os **oito padrões de sinalização** propostos pelo protocolo:

- **Título e linha fina** com correções: passe o cursor sobre as palavras coloridas ("Irã" em índigo, "sexta-feira" em vermelho) — o ícone ✎ indica correção.
- **Corpo da matéria** com erratas colapsáveis por baixo dos parágrafos: cada errata tem título, motivo, comparativo antes/depois e data/hora da alteração.
- **Bloco amarelo de conteúdo novo**: aparecem em pontos da matéria com informações acrescentadas após a publicação inicial.
- **Aba de Correções**: no topo da matéria, clique na aba "Correções" para ver todas as erratas da cobertura, com filtros por tipo.
- **Legenda visual**: no sidebar direito, veja o significado de cada cor.
- **Botão de comunicar erro**: no fim da matéria, clique em "Reportar erro" para ver o modal de comunicação com o leitor.

## Testar o comportamento de 24 horas

Adicione `?simular=25h` à URL para ver o estado da matéria depois das 24 horas:

```
index.html?simular=25h
```

Outras opções: `+2h`, `+12h`, `+23h`, `+72h`. Também há atalhos clicáveis no banner discreto que aparece no topo da matéria.

**O que muda depois de 24h:**

- As caixas amarelas de "conteúdo novo" perdem a marcação (o texto fica no fluxo natural do artigo)
- Os selos "NOVO · acrescentado há Xh" somem
- O bloco de "trecho excluído" desaparece por completo
- Correções (factuais, grafia, imprecisão, retificação) e direito de resposta **permanecem sempre**

## Voltar ao índice

Volte à [página principal do protótipo](../) para ver as duas versões (PT e EN) e a descrição do projeto.
