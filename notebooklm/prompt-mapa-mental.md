# Prompt reutilizável — mapa mental com evidências

Este prompt adapta as diretrizes da nota “Ben Carson — Segundo Cérebro” para organizar uma revisão no NotebookLM. É um roteiro reutilizável; sua presença no repositório não significa, por si só, que esta versão foi executada. Os testes efetivamente realizados são documentados em [engenharia de prompts](../docs/prompts.md).

Antes de usar, selecione as fontes pertinentes no caderno e substitua os campos entre colchetes.

## Prompt principal

```text
Crie um mapa mental de estudo sobre [tema ou episódio] a partir exclusivamente
das fontes selecionadas neste caderno.

Objetivo da revisão: [o que quero compreender ou conseguir explicar].
Público: estudante que deseja revisar o tema e conferir as evidências.

Organize o mapa em até seis ramos:
1. Trajetória e contexto.
2. Aprendizagem e THINK BIG, quando houver evidência pertinente.
3. Decisões e incerteza.
4. Equipe e execução.
5. Carreira e reflexão.
6. Fontes, divergências e lacunas.

Use no máximo três subitens por ramo e frases curtas. Se um ramo não for
sustentado pelas fontes, indique isso ou proponha sua exclusão.

Para cada afirmação factual, forneça uma citação verificável do caderno.
Identifique título da fonte e página ou seção quando disponíveis. Não invente
referências, páginas, citações literais, acontecimentos ou pensamentos privados.

Escolha o tipo de fonte conforme a pergunta: relato autobiográfico para a
narrativa pessoal; entrevista para declarações contextualizadas; documentação
institucional para registros; artigo original para métodos e resultados.
Não aplique uma hierarquia universal entre esses tipos.

Separe:
- informação apresentada pela fonte;
- interpretação proposta para estudo;
- informação não documentada ou divergente.

Se analisar uma decisão, use o roteiro:
problema → informações → alternativas → riscos → decisão → execução →
resultado → aprendizado.
Não preencha etapas ausentes por suposição. Diferencie a lição declarada
pelo autor da reflexão de quem estuda.

As ligações do mapa devem representar relações temáticas. Só descreva causa
e efeito quando houver suporte suficiente e explicite a natureza desse suporte.
Trate THINK BIG como o modelo pessoal apresentado nas fontes. Situe os
episódios médicos em seu contexto histórico, sem produzir orientação clínica.

Entregue:
A. Um mapa em lista hierárquica, com as citações junto dos subitens.
B. Uma tabela curta: afirmação | fonte | tipo de informação | limite.
C. Até três lacunas prioritárias e perguntas para investigá-las.
D. Cinco perguntas de revisão que possam ser respondidas a partir do mapa.

Quando não houver evidência suficiente, escreva “não documentado nas fontes
selecionadas” e explique qual informação seria necessária.
```

## Variações para revisar a resposta

**Reduzir o mapa sem perder rastreabilidade**

```text
Reduza o mapa anterior a cinco ramos e dois subitens por ramo. Preserve as
citações e as distinções entre evidência, interpretação e lacuna. Liste ao final
os temas retirados para que eu possa decidir se precisam voltar.
```

**Verificar relações e evidências**

```text
Revise cada ligação do mapa anterior. Indique se ela representa associação
temática, sequência temporal ou uma afirmação causal. Confira as referências
das afirmações factuais. Reescreva as ligações que excedem a evidência e
mantenha explícitas as divergências que não puder resolver.
```

**Preparar uma versão Mermaid para o GitHub**

```text
Converta apenas a estrutura central do mapa em um diagrama Mermaid flowchart
TD, com no máximo oito nós e rótulos curtos. Use linhas sem setas para relações
temáticas. Fora do diagrama, apresente uma legenda com as fontes de cada ramo.
Não remova qualificações necessárias nem apresente a estrutura como causal.
```

## Conferência antes de publicar

Abra as citações e verifique as principais afirmações. Ao levar a resposta ao GitHub, associe as referências do caderno a links ou identificadores legíveis na [curadoria](../sources/fontes.md); marcadores internos do chat, sozinhos, não permitem ao leitor localizar a evidência. Registre o prompt utilizado, a resposta obtida e qualquer correção feita na revisão.
