# Ben Carson — Segundo Cérebro com NotebookLM

**Caderno temático sobre aprendizagem, pensamento crítico e tomada de decisão, desenvolvido para o desafio de projeto da DIO.**

Autor: [Augusto Lopes Lyra](https://github.com/lopeslyra10) · Documentação e experimentos: **20/09/2026**

[Abrir o caderno Ben Carson Brain](https://notebook.google.com/notebook/068a9fb7-57e7-482a-b3da-a12a735c08ae) · [Ler o miniguia](docs/miniguia.md) · [Ver os testes reais](docs/prompts.md)

## Contexto e objetivos

O tema escolhido é a trajetória de Ben Carson como estudante, médico e tomador de decisões. A pergunta central é: **como transformar uma narrativa biográfica em conhecimento organizado, verificável e útil para estudar?**

O projeto usa o NotebookLM como apoio à aprendizagem ativa: formular perguntas, comparar respostas, conferir referências e registrar limites. O termo “segundo cérebro” descreve a organização externa de notas e conexões; não significa reproduzir a mente de Carson.

Os objetivos de estudo são:

1. Organizar os principais eixos da trajetória e da aprendizagem de Carson.
2. Distinguir relato pessoal, documentação institucional, resultado científico e interpretação de estudo.
3. Analisar leitura, preparação, colaboração e decisão sem transformar uma biografia em prova de causalidade.
4. Testar prompts, conferir suas respostas e registrar o que precisou ser corrigido.
5. Produzir resumos, glossário, mapa de conhecimento e perguntas reutilizáveis para revisão.

O recorte é educacional e histórico. Os episódios médicos são estudados como documentos e exemplos de análise de evidências, sem estabelecer condutas clínicas atuais.

## O que está publicado

O caderno existente continha **30 fontes** e a nota **“Ben Carson — Segundo Cérebro”** quando foi conferido. Esta entrega seleciona **cinco fontes abertas em texto**, já presentes nele, para um recorte reproduzível. Os três experimentos foram executados com essas cinco fontes selecionadas.

O GitHub reúne a documentação e o material de estudo em Markdown. O caderno interativo continua no serviço do Google; o acesso ao link depende das permissões do notebook e pode exigir login. A leitura deste repositório é independente desse acesso.

| Requisito do desafio | Entrega |
|---|---|
| Contexto e objetivos | Esta página |
| Curadoria de 3 a 5 fontes abertas | [Cinco referências, critérios e limitações](sources/fontes.md) |
| Perguntas e variações de prompts | [Três testes realizados e biblioteca de revisão](docs/prompts.md) |
| Respostas, referências e dificuldades | [Registro dos testes](docs/prompts.md) e [troubleshooting](docs/troubleshooting.md) |
| Resumos estruturados e glossário | [Miniguia de estudo](docs/miniguia.md) |
| Organização do conhecimento | [Knowledge Map](docs/knowledge-map.md) e [nota-base adaptada](notebooklm/nota-base.md) |
| Prompt de mapa mental | [Instruções reutilizáveis](notebooklm/prompt-mapa-mental.md) |

## Curadoria em cinco fontes

| ID | Fonte | Papel no estudo |
|---|---|---|
| F1 | [Academy of Achievement — perfil e entrevistas](https://achievement.org/achiever/benjamin-s-carson/) | Narrativa pessoal e princípios de aprendizagem |
| F2 | [Dialogue — entrevista de 1990](https://www.dialogue.adventist.org/2360/ben-carson-dialogue-with-an-adventist-neurosurgeon) | Formação, valores e preparação |
| F3 | [Dialogue — entrevista de 2003](https://dialogue.adventist.org/949/ben-carson-dialogue-with-a-pediatric-neurosurgeon-who-despite-surgery-for-cancer-still-thinks-big) | Experiência pessoal e perspectiva sobre o cuidado |
| F4 | [Johns Hopkins — Benjamin S. Carson Collection](https://medicalarchivescatalog.jhmi.edu/ArchivEra/Portal/Default.aspx?component=AABC&record=26894498-4188-47df-bf26-2460614f4321) | Cronologia e descrição institucional |
| F5 | [PubMed — Hemispherectomy: a hemidecortication approach and review of 52 cases](https://pubmed.ncbi.nlm.nih.gov/8847583/) | Resumo científico histórico e limites de generalização |

“Aberta” significa disponível para leitura gratuita. F5 oferece metadados e resumo, não comprovação de acesso ao artigo integral. Autoria, datas, justificativas e vieses estão nas [fichas das fontes](sources/fontes.md).

## Método e resultados da experimentação

O ciclo adotado foi **perguntar → localizar a referência → conferir o trecho → reformular → sintetizar → revisar sem consulta**.

O primeiro prompt produziu uma síntese com citações, mas usou linguagem geral para afirmações pessoais. O segundo pediu classificação das evidências e limites em uma tabela. O terceiro auditou uma estatística do resumo científico e mostrou por que é necessário conferir denominadores e categorias do resultado. A análise completa, inclusive uma imprecisão remanescente, está no [registro de prompts](docs/prompts.md).

Os testes foram conduzidos nesta etapa de conclusão do projeto. Não se atribuem experimentos ou respostas ao histórico do chat anterior. O registro público contém prompts exatos, trechos curtos e sínteses identificadas; não é uma transcrição integral do caderno.

## Como estudar com este material

1. Leia as [fichas das fontes](sources/fontes.md) e o [miniguia](docs/miniguia.md).
2. Use o [mapa de conhecimento](docs/knowledge-map.md) para escolher um tema.
3. No caderno, selecione F1–F5 pelos títulos e reutilize um [prompt de revisão](docs/prompts.md).
4. Responda às perguntas por conta própria antes de pedir a correção da IA.
5. Abra as citações e registre dúvidas ou divergências, em vez de aceitar a resposta só porque parece bem escrita.

Para reproduzir o estudo em outro caderno, adicione as cinco URLs como fontes, confira o texto importado e aplique os prompts. A [ajuda oficial do Google](https://support.google.com/notebooklm/answer/16206563?hl=pt-BR) explica o funcionamento de fontes, conversa e notas. Na interface consultada, o produto aparece como “Gemini Notebook”; o nome NotebookLM foi mantido aqui por ser o nome usado no desafio.

## Estrutura

```text
ben-carson-second-brain-notebooklm/
├── README.md
├── docs/
│   ├── knowledge-map.md
│   ├── miniguia.md
│   ├── prompts.md
│   └── troubleshooting.md
├── notebooklm/
│   ├── nota-base.md
│   └── prompt-mapa-mental.md
├── sources/
│   └── fontes.md
└── assets/
    └── README.md
```

## Autoria, transparência e direitos autorais

A seleção temática e o caderno pertencem ao autor do projeto. A organização editorial, a revisão de fontes e a documentação foram concluídas com assistência de IA. Os fatos devem ser verificados nas referências, e as aplicações de estudo estão identificadas como propostas do projeto.

*Gifted Hands* faz parte do contexto de estudo pessoal. Seu PDF integral não é publicado. Este repositório contém links, notas e sínteses próprias, sem transferir direitos de obras de terceiros. Não se afirma que registros de catálogo importados equivalem ao texto completo de um livro.
> Caderno temático sobre Ben Carson com NotebookLM, voltado à aprendizagem ativa e ao pensamento crítico. Reúne cinco fontes abertas, três testes reais de prompts com análise das respostas, registro de dificuldades, miniguia com glossário e mapa de conhecimento. O projeto diferencia relatos pessoais, fatos institucionais e evidências científicas.
