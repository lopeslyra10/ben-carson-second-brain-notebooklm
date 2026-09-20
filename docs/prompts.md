# Engenharia de prompts e registro de experimentos

## Condições e evidências

**Execução real:** 20/09/2026, no caderno [Ben Carson Brain](https://notebook.google.com/notebook/068a9fb7-57e7-482a-b3da-a12a735c08ae), pela interface web. O início da sequência foi exibido como 12:33, horário de Brasília. Foram selecionadas somente as cinco fontes [F1–F5](../sources/fontes.md), entre as 30 existentes. Os testes T1, T2 e T3 ocorreram na mesma conversa; T2 e T3 dependem do histórico anterior.

Os comandos abaixo são os textos efetivamente enviados. As respostas são documentadas por **trechos curtos e sínteses editoriais**, com análise separada. Os números de citação são os que apareceram em cada resposta; podem mudar em outra execução e não são os IDs F1–F5. Referências pelo título e URL permitem reencontrar o documento.

Não foram recuperados registros de experimentos do chat anterior. Esta sequência foi realizada para concluir o projeto e não deve ser apresentada como atividade anterior do autor.

## T1 — Síntese aberta

**Pergunta estratégica:** quais temas a IA prioriza quando recebe uma pergunta ampla?

```text
Resuma em até 120 palavras o que a trajetória de Ben Carson ensina sobre aprendizagem e tomada de decisão. Cite as fontes.
```

**Resposta observada — síntese:** associou leitura, esforço e confiança à aprendizagem; apresentou uma forma de avaliar riscos e mencionou preparação. A leitura foi descrita como “de forma muito superior à televisão”.

**Referências exibidas:** citações 1 e 4 apontaram para a entrevista de 1990 [F2](https://www.dialogue.adventist.org/2360/ben-carson-dialogue-with-an-adventist-neurosurgeon); 7, 8, 9 e 10 apontaram para [F1](https://achievement.org/achiever/benjamin-s-carson/). Havia controles de expansão para outras citações; não se afirma aqui ter auditado todos os trechos ocultos.

**Avaliação:** trouxe referências, mas apresentou afirmações do entrevistado com linguagem de regra geral. A presença de uma citação não demonstrava a causalidade sugerida. O resultado serviu para levantar temas; exigiu revisão antes de entrar no miniguia.

**Mudança para T2:** exigir natureza da evidência, fonte e limite em cada linha.

## T2 — Classificação e limites

**Pergunta estratégica:** a resposta melhora quando cada afirmação precisa declarar o que a sustenta?

```text
Reformule a resposta anterior em uma tabela com exatamente 3 linhas e até 120 palavras: afirmação | tipo de evidência | fonte | limite. Separe relato de Carson, fato institucional e resultado de pesquisa. Não trate superioridade da leitura, crescimento da inteligência ou fé como causalidade científica demonstrada. Use uma linha de entrevista, uma do catálogo Benjamin S. Carson Collection e uma do resumo de Hemispherectomy: a hemidecortication approach and review of 52 cases. Cite cada linha. Se faltar evidência, diga não informado.
```

**Resposta observada — síntese por linha:**

| Linha | O que a resposta entregou | Referência exibida |
|---|---|---|
| Relato | Atribuiu a Carson as mudanças pessoais narradas e escreveu “Causalidade científica não demonstrada”. | Citações 1 e 2 → [F2](https://www.dialogue.adventist.org/2360/ben-carson-dialogue-with-an-adventist-neurosurgeon) |
| Instituição | Apontou atuação profissional, sem inferir o processo decisório pelo cargo. | Citação 3 → [F4](https://medicalarchivescatalog.jhmi.edu/ArchivEra/Portal/Default.aspx?component=AABC&record=26894498-4188-47df-bf26-2460614f4321) |
| Pesquisa | Resumiu o resultado como controle de crises em 96% dos sobreviventes e indicou que o estudo não avalia aprendizagem. | Citações 4 e 5 → [F5](https://pubmed.ncbi.nlm.nih.gov/8847583/) |

**Avaliação:** a tabela criou uma distinção útil entre tipos de informação e manteve três linhas. Porém, a estatística ficou comprimida: “controle” não explicava as categorias combinadas. A expressão “casos pediátricos” também era mais específica que a caracterização de toda a amostra disponível no resumo. O número precisava de auditoria, não de repetição automática.

**Mudança para T3:** restringir a resposta ao abstract e exigir definição do resultado, denominador e limites.

## T3 — Auditoria de uma afirmação

**Pergunta estratégica:** o que exatamente uma porcentagem mede e o que fica fora dela?

```text
Audite somente a linha do estudo de 52 casos da resposta anterior. Usando exclusivamente o resumo de Hemispherectomy: a hemidecortication approach and review of 52 cases, responda em até 130 palavras: 1) o que exatamente significa 96%, qual o denominador descrito e quais categorias foram combinadas; 2) período da série e mortalidade relatada; 3) o que esse resumo NÃO permite concluir. Não acrescente dados do texto integral nem recomendações atuais. Cite a fonte.
```

**Resposta observada — síntese:** identificou 46 de 48 sobreviventes, reunindo ausência ou redução de crises; situou a série em 1975–1994 e mencionou três mortes perioperatórias e uma posterior. Também negou que o resumo estabelecesse eficácia comparativa ou explicasse a aprendizagem de Carson. Todas as citações visíveis dessa resposta usaram o número 1 para [F5](https://pubmed.ncbi.nlm.nih.gov/8847583/).

**Conferência realizada:** foi aberto o texto da fonte F5 dentro do notebook, na seção **Abstract**. Ela estava efetivamente importada e continha o resultado agrupado. O denominador numérico 48 é uma reconstrução aritmética de 52 menos quatro mortes, coerente com 46/48 ≈ 96%; o resumo usa a expressão pacientes sobreviventes.

**Imprecisão remanescente:** a resposta chamou ausência de crises de “cura total”. Essa equivalência não foi adotada no material final. A condição descrita no resumo se refere ao último acompanhamento, não a uma garantia permanente. Mesmo uma resposta de auditoria precisa ser conferida.

**Decisão editorial:** manter a pesquisa como exercício de leitura crítica, sem converter essa porcentagem em expectativa individual ou recomendação médica.

## O que mudou entre os prompts

| Versão | Ganho observado | Limitação remanescente |
|---|---|---|
| T1: tema + síntese + citações | Levantamento rápido de assuntos | Atribuição insuficiente de opiniões e relatos |
| T2: tabela + tipo + limite | Separação explícita de evidências | Compressão de resultado quantitativo |
| T3: uma afirmação + uma fonte + escopo | Resultado mais verificável | Terminologia ainda exigiu revisão |

Não se trata de avaliação estatística do modelo. São três observações de uma única sequência; não há garantia de respostas idênticas em novas execuções. A configuração do modelo e eventuais instruções internas do serviço não foram exportadas.

## Prompts reutilizáveis para próximas revisões

**Status:** os modelos abaixo são propostas para uso futuro; não são apresentados como novos testes executados. Substitua os campos entre colchetes e selecione as fontes adequadas antes de enviar.

### P1 — Síntese rastreável

```text
Com base somente nas fontes selecionadas, explique [tema] em até 200 palavras. Para cada ponto, indique fonte e seção, classifique como relato, fato documentado, resultado científico ou inferência. Declare o que não foi possível determinar. Não invente páginas ou citações.
```

### P2 — Perguntas antes da resposta

```text
Faça 5 perguntas sobre [tema], uma por vez. Espere minha resposta antes de corrigir. Depois compare com as fontes, explique a lacuna e mostre a referência. Não revele o gabarito antes da minha tentativa.
```

### P3 — Comparação de versões

```text
Compare [afirmação] em [fonte A] e [fonte B]. Mostre concordâncias, divergências e informações ausentes. Considere data, contexto e possível dependência entre as fontes. Não escolha uma versão apenas pela quantidade de repetições.
```

### P4 — Reconstrução de decisão

```text
Organize [episódio] em problema, informações disponíveis, alternativas, riscos, decisão, execução e resultado. Cite cada etapa e marque como não informado o que não aparece. Separe o que Carson disse da interpretação que podemos propor; não invente intenções privadas.
```

### P5 — Auditoria de números

```text
Confira [afirmação quantitativa] na fonte selecionada. Identifique população, numerador, denominador, definição do resultado, período e seguimento. Separe valores expressos no texto de cálculos seus. Não equipare melhora, ausência de sintomas e cura.
```

### P6 — Glossário com exemplos

```text
Crie um glossário de 8 termos sobre [tema]. Para cada um, dê definição simples, exemplo original de estudo e uma confusão comum. Cite a fonte quando a definição depender do documento e identifique os exemplos como criações didáticas.
```

### P7 — Checagem final

```text
Revise minha síntese: [colar texto]. Liste apenas afirmações sem suporte, generalizações, divergências omitidas e referências inadequadas. Para cada problema, proponha uma formulação mais precisa ou indique a fonte adicional necessária. Não preencha as lacunas por suposição.
```

Para organização visual, use o [prompt de mapa mental](../notebooklm/prompt-mapa-mental.md). Para revisão prática, use o [miniguia](miniguia.md).

[Voltar ao projeto](../README.md)
