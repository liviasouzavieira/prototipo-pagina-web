# Protótipo de página web — Protocolo de correção de erros no jornalismo digital

**Uma matéria fictícia sobre um conflito diplomático (o "conflito no Irã") demonstra, em contexto real de leitura, todos os padrões visuais e comportamentais do protocolo de correção de erros no jornalismo digital.**

O protótipo está disponível em duas versões espelhadas: **português** (`pt/`) e **inglês** (`en/`). As duas mostram a mesma cobertura, com os mesmos padrões de sinalização — o que muda é apenas o idioma dos textos.

---

## 👉 Ver o protótipo funcionando

- 🇧🇷 [Versão em português](pt/) — cobertura fictícia da reunião emergencial da ONU sobre o conflito no Irã
- 🇺🇸 [English version](en/) — fictional coverage of the U.N. Security Council emergency session on the Iran conflict

Se o site já estiver publicado via GitHub Pages, os links acima levam direto para a matéria completa.

---

## Sobre a pesquisa

Este protótipo é resultado da pesquisa **"Protocolo de gestão para correção de erros no jornalismo digital"** (nº PPP0014/2024 — Edital Fapesb/CNPq — Programa Primeiros Projetos 004/2023). Está em estado de protótipo funcional.

**Pesquisadora responsável:** Lívia de Souza Vieira ([livia.vieira@ufba.br](mailto:livia.vieira@ufba.br))

---

## O que o protótipo demonstra

O protótipo é uma matéria fictícia de um veículo jornalístico, com o layout comum a sites de notícia: cabeçalho, banner ao vivo, abas de navegação, texto em destaque, colunas de análise, cobertura ao vivo, redes sociais e comentários. O diferencial é que **cada tipo de alteração pós-publicação está marcado com um padrão visual próprio**, seguindo a taxonomia proposta pelo protocolo:

- **Erro factual** (vermelho) — corrigido no primeiro parágrafo da matéria em destaque
- **Erro de grafia** (índigo) — corrigido no título e em outro trecho da linha do tempo
- **Correção por imprecisão** (laranja) — corrigido em número aproximado que virou cifra exata
- **Retificação em declaração** (roxo) — corrigido em fala mal transcrita da embaixadora
- **Direito de resposta** (teal) — bloco permanente com resposta do senador Carlos Mendes
- **Trecho excluído** (cinza tracejado) — bloco que se autodestrói após 24 horas
- **Conteúdo novo** (amarelo) — caixas amarelas que perdem a marcação após 24 horas

Além disso, o protótipo tem:

- **Legenda visual** no sidebar explicando cada cor
- **Aba dedicada de Correções** (Errata) com filtros por tipo
- **Sistema de comunicação de erro** pelo leitor (modal com formulário)
- **Botões de simulação de 24 horas** no topo, para você ver na hora o "depois" das marcações voláteis

---

## Como testar o comportamento de 24 horas

O protótipo simula um relógio ficcional para permitir que você veja o "antes" e o "depois" das 24 horas **sem esperar de verdade**. Adicione um parâmetro à URL:

```
pt/?simular=25h    → simula o estado da matéria 25 horas depois
en/?simulate=25h   → mesmo comportamento em inglês
```

Alternativas úteis: `+2h`, `+12h`, `+23h`, `+72h`. Em qualquer versão simulada, aparece um banner discreto no topo com atalhos para navegar entre janelas de tempo.

**Resultado esperado:**

- Antes de 24h: caixas amarelas de conteúdo novo visíveis, bloco de trecho excluído no fim da matéria, todas as marcações ativas.
- Depois de 24h: o amarelo some (o texto fica integrado ao corpo, sem marcação); o bloco de trecho excluído desaparece por completo; correções e direito de resposta permanecem.

---

## Plugin instalável em qualquer CMS

O vocabulário visual demonstrado neste protótipo foi transformado em um **plugin autocontido**, pronto para instalação em WordPress, Ghost, Drupal ou qualquer outro sistema de gestão de conteúdo, no repositório companheiro:

👉 [github.com/liviasouzavieira/plugin-correcao-erros-jornalismo-digital](https://github.com/liviasouzavieira/plugin-correcao-erros-jornalismo-digital)

---

## Como citar

Se você usar este protótipo em pesquisa acadêmica, ensino ou produção editorial, cite a pesquisa que o originou:

```
VIEIRA, Lívia de Souza. Protocolo de gestão para correção de erros no
jornalismo digital. Salvador: Fapesb/CNPq, 2026. (Programa Primeiros
Projetos, Edital 004/2023, nº PPP0014/2024).
```

---

## Licença

Distribuído sob a licença **MIT** — veja [LICENSE](LICENSE) para os termos completos. Uso comercial e adaptação são permitidos, com atribuição.

---

## Instruções por idioma

- 🇧🇷 [Documentação em português](pt/README-pt.md)
- 🇺🇸 [English documentation](en/README-en.md)
