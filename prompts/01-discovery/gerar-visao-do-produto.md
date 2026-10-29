# Prompt 01 — Geração da Visão do Produto

## 1. Identificação

- **ID:** PROMPT-DISC-001
- **Etapa:** Descoberta e visão do produto
- **Artefato de saída:** `docs/01-discovery/visao-do-produto.md`
- **Idioma de saída:** Português brasileiro
- **Tipo:** Geração de documento de negócio e produto

## 2. Objetivo

Gerar o documento de visão do produto de um projeto de desenvolvimento de aplicação de Machine Learning assistido por LLMs.

O documento deverá estabelecer o contexto do problema, a proposta de valor, os usuários, os objetivos, o escopo preliminar, as restrições e os critérios iniciais de sucesso. Deverá servir como referência para as etapas posteriores de engenharia de requisitos, arquitetura e implementação.

## 3. Contexto do projeto

O projeto faz parte de um mestrado profissional em Inteligência Computacional Aplicada às Decisões Financeiras.

O objetivo é desenvolver uma aplicação web funcional, baseada em Machine Learning, com qualidade técnica suficiente para constituir um protótipo de solução de negócio com potencial de evolução comercial.

A hipótese inicial é uma aplicação de apoio à avaliação de risco de crédito, utilizando uma base de dados pública do Kaggle. A escolha definitiva do problema e da base ainda deverá ser validada.

O desenvolvimento será realizado inicialmente com o auxílio do Antigravity. O processo de engenharia deverá ser documentado em arquivos Markdown versionados, incluindo prompts, especificações, decisões técnicas, instruções de execução, testes e evidências.

O repositório deverá permitir que terceiros tentem reproduzir o desenvolvimento utilizando os mesmos artefatos, inclusive em outros LLMs e ambientes de desenvolvimento.

O projeto possui, portanto, dois resultados principais:

1. Uma aplicação de Machine Learning com funcionalidades verificáveis e potencial de evolução comercial.
2. Um processo documentado de desenvolvimento assistido por LLM, cuja reprodutibilidade e qualidade poderão ser investigadas.

## 4. Instruções para geração

Com base exclusivamente nas informações disponíveis e em inferências claramente identificadas, produza um documento de visão do produto que:

1. Explique o contexto e a motivação do projeto.
2. Defina o problema de negócio preliminar que se pretende investigar.
3. Identifique os usuários e suas necessidades, distinguindo usuários confirmados de públicos hipotéticos.
4. Apresente a proposta de valor e os benefícios esperados.
5. Estabeleça o objetivo geral e os objetivos específicos do produto.
6. Delimite o escopo inicial e os itens explicitamente fora de escopo.
7. Descreva as principais capacidades esperadas da aplicação, sem transformá-las prematuramente em requisitos técnicos detalhados.
8. Defina critérios iniciais de sucesso que possam ser verificados posteriormente.
9. Identifique restrições, riscos, dependências e questões em aberto.
10. Diferencie os objetivos do produto dos objetivos experimentais relacionados ao desenvolvimento assistido por LLM.
11. Considere a qualidade de software, a confiabilidade das previsões, a segurança, a interpretabilidade e a rastreabilidade como aspectos relevantes.
12. Trate a possibilidade de evolução comercial como objetivo de engenharia, sem afirmar que o protótipo estará automaticamente apto para produção.

## 5. Estrutura obrigatória do documento de saída

O documento deverá conter, nesta ordem:

1. Identificação do documento
2. Contexto e motivação
3. Problema de negócio
4. Visão do produto
5. Usuários e necessidades
6. Proposta de valor
7. Objetivos do produto
8. Escopo preliminar
9. Capacidades esperadas
10. Critérios iniciais de sucesso
11. Restrições e premissas
12. Riscos e questões em aberto
13. Relação com o experimento de desenvolvimento assistido por LLM
14. Condições para evolução comercial

## 6. Regras de qualidade

- Não invente entrevistas, pesquisas de mercado, dados estatísticos, resultados ou validações que não tenham sido fornecidos.
- Não apresente a escolha da avaliação de crédito como definitiva antes de sua validação.
- Não selecione uma base de dados, algoritmo, linguagem, framework ou arquitetura sem que essa decisão tenha sido solicitada ou formalizada.
- Não confunda previsão de risco com decisão automática de concessão ou negação de crédito.
- Não prometa explicabilidade completa ou ausência de vieses.
- Diferencie fatos conhecidos, hipóteses, decisões provisórias e questões em aberto.
- Formule critérios de sucesso verificáveis, evitando expressões vagas como "sistema eficiente" sem indicar como a eficiência será avaliada.
- Utilize linguagem profissional, objetiva e adequada a um projeto acadêmico de caráter aplicado.
- Escreva em português brasileiro, utilizando Markdown.
- Não inclua código de implementação.
- Não gere requisitos detalhados nem substitua os documentos das etapas posteriores.

## 7. Instrução final

Produza somente o conteúdo completo do arquivo `visao-do-produto.md`.

Antes de concluir, verifique se todas as seções obrigatórias estão presentes, se as hipóteses estão identificadas e se nenhuma decisão ainda não tomada foi apresentada como fato confirmado.

Quando faltarem informações, registre a lacuna e seus possíveis impactos, em vez de preencher a ausência com suposições arbitrárias.
