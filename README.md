# LLM-Driven ML Application Engineering

**Engenharia de aplicações de Machine Learning assistida por LLMs: qualidade de software, rastreabilidade e reprodutibilidade.**

## 1. Sobre o projeto

Este repositório documenta o desenvolvimento de uma aplicação web baseada em Machine Learning, utilizando Modelos de Linguagem de Grande Escala (LLMs) como agentes de apoio à engenharia de software.

O projeto é desenvolvido no contexto de um mestrado profissional em Inteligência Computacional Aplicada às Decisões Financeiras e tem como propósito investigar como um processo estruturado, especificado e versionado em arquivos Markdown pode orientar o desenvolvimento de soluções computacionais com qualidade técnica e potencial de aplicação profissional.

A proposta vai além da geração de código ou da implementação isolada de algoritmos de aprendizado de máquina. Busca-se construir um protótipo funcional de solução de negócio, com arquitetura organizada, requisitos verificáveis, validação experimental, documentação técnica e condições para evolução futura em direção a uma solução comercial.

A aplicação inicial proposta é um sistema de apoio à avaliação de risco de crédito, cuja definição definitiva dependerá da análise e da seleção de uma base de dados pública adequada.

Paralelamente, o próprio processo de desenvolvimento será tratado como objeto de documentação e investigação. Prompts, especificações, decisões técnicas, instruções de execução, testes e evidências serão organizados para permitir que terceiros tentem reproduzir o projeto utilizando os mesmos artefatos, inclusive em diferentes LLMs e ambientes de desenvolvimento (*harnesses*).

## 2. Objetivos

### 2.1. Objetivo geral

Desenvolver uma aplicação de Machine Learning com potencial de evolução para uma solução comercial, utilizando um processo de engenharia de software assistido por LLMs, documentado e reproduzível, e investigar a qualidade dos resultados obtidos em diferentes condições de execução.

### 2.2. Objetivos específicos

- Identificar e estruturar um problema concreto relacionado à tomada de decisão financeira.
- Selecionar e analisar uma base de dados pública adequada à solução proposta.
- Desenvolver e avaliar modelos de Machine Learning segundo critérios estatísticos e técnicos apropriados.
- Projetar uma aplicação web que disponibilize as funcionalidades do modelo de maneira utilizável, consistente e verificável.
- Documentar requisitos, arquitetura, contratos entre componentes, especificações técnicas e critérios de aceitação.
- Estruturar prompts, instruções, *skills* e eventuais agentes para orientar a geração e a validação dos artefatos.
- Estabelecer mecanismos de rastreabilidade entre as necessidades do negócio, os requisitos, o código implementado e os testes.
- Avaliar a qualidade da aplicação como produto de software, e não apenas o desempenho preditivo do modelo.
- Permitir que outros usuários tentem reproduzir o desenvolvimento a partir da documentação publicada.
- Investigar diferenças de qualidade entre execuções, usuários, LLMs e ambientes de desenvolvimento.

## 3. Visão do produto: protótipo com potencial de evolução comercial

A aplicação deverá ser concebida como um protótipo de solução tecnológica para um problema real, e não como uma demonstração isolada de um algoritmo de aprendizado de máquina.

Considerando a hipótese inicial de avaliação de crédito, o sistema poderá oferecer funcionalidades como:

- Recebimento e validação dos dados necessários à análise.
- Estimativa do risco de inadimplência por meio de um modelo treinado.
- Apresentação de probabilidades estimadas, classificações e informações relevantes para a interpretação dos resultados.
- Visualização de métricas de desempenho e limitações conhecidas do modelo.
- Simulação de cenários para investigar como alterações nas entradas afetam as previsões.
- Registro das versões do modelo e dos parâmetros relevantes para a rastreabilidade das inferências.
- Disponibilização dos recursos por meio de uma interface web e de uma API, caso essa arquitetura seja confirmada durante o planejamento.

Essas funcionalidades representam possibilidades iniciais, que serão refinadas a partir do documento de visão, dos requisitos e da análise da base de dados.

### 3.1. Critérios de qualidade do produto

O desenvolvimento deverá considerar, de forma integrada:

- **Qualidade preditiva:** desempenho avaliado com métricas apropriadas ao problema e aos custos dos diferentes tipos de erro.
- **Qualidade de software:** organização modular, legibilidade, testabilidade, tratamento de erros e separação de responsabilidades.
- **Usabilidade:** apresentação compreensível dos resultados e interação coerente com as necessidades do usuário.
- **Interpretabilidade:** recursos adequados para investigar as previsões e suas limitações.
- **Segurança e proteção de dados:** validação de entradas, controle de exposição de informações e tratamento adequado dos dados utilizados.
- **Rastreabilidade:** identificação dos dados, versões dos modelos, configurações e evidências de validação.
- **Reprodutibilidade:** documentação suficiente para reconstruir o ambiente e executar novamente os procedimentos definidos.
- **Manutenibilidade e evolução:** arquitetura que permita substituir modelos, corrigir componentes e incorporar novas funcionalidades sem reconstruir integralmente o sistema.

A qualidade não será presumida a partir da geração bem-sucedida do código. Deverá ser demonstrada por meio de testes, métricas, critérios de aceitação e evidências documentadas.

### 3.2. Limites da proposta comercial

O objetivo é alcançar um protótipo tecnicamente consistente e com potencial de evolução comercial. Isso não equivale a afirmar que o sistema estará pronto para uso irrestrito em produção.

Uma implantação comercial efetiva poderá exigir validação adicional com dados representativos, avaliação de vieses e impactos, controles de segurança, requisitos regulatórios aplicáveis, monitoramento do modelo, governança operacional e outros mecanismos determinados pelo contexto de utilização.

No caso de avaliação de crédito, a previsão será tratada como informação de apoio à decisão. Não se presumirá que uma probabilidade estimada, isoladamente, seja suficiente para aprovar ou negar crédito.

## 4. Engenharia de software assistida por LLMs

O desenvolvimento será orientado por um pipeline documentado, no qual cada etapa deverá produzir artefatos verificáveis que sirvam de entrada para as etapas seguintes.

O processo deverá contemplar descoberta do problema, seleção de dados, especificação do experimento de Machine Learning, engenharia de requisitos, arquitetura, planejamento da implementação, geração de código, testes e validação.

Os LLMs serão utilizados como instrumentos de apoio à análise, à especificação, à implementação e à revisão. Suas saídas deverão ser avaliadas segundo critérios explícitos, evitando que a aceitação de um artefato dependa exclusivamente da confiança na resposta do modelo.

O ambiente inicial de desenvolvimento será o Antigravity. A utilização de *skills*, agentes e automações será definida conforme as necessidades técnicas identificadas durante o projeto.

## 5. Investigação de reprodutibilidade

O repositório também servirá como base para uma investigação exploratória sobre a capacidade de reproduzir uma aplicação a partir de um processo de desenvolvimento documentado.

Serão consideradas, conforme a viabilidade, três situações:

1. Reexecução do pipeline no ambiente original.
2. Reprodução por outros usuários, utilizando os mesmos artefatos e instruções.
3. Reprodução utilizando outros LLMs e ambientes de desenvolvimento.

A avaliação deverá considerar tanto a qualidade do produto gerado quanto a fidelidade ao processo especificado.

Entre os critérios de comparação estão:

- Conformidade com os requisitos e critérios de aceitação.
- Funcionamento e completude das funcionalidades.
- Qualidade, organização e manutenibilidade do código.
- Cobertura e resultados dos testes.
- Correção do pipeline de dados e de Machine Learning.
- Validade das métricas e do protocolo de avaliação.
- Clareza e completude da documentação.
- Facilidade de instalação, execução e reprodução.
- Quantidade e natureza das intervenções humanas necessárias.

Sempre que possível, serão registradas as versões dos modelos e das ferramentas, as configurações relevantes, os prompts utilizados, os resultados dos testes e as alterações realizadas durante cada execução.

O objetivo não é exigir código idêntico entre execuções, mas investigar em que medida diferentes condições de desenvolvimento podem produzir soluções funcionalmente equivalentes, tecnicamente adequadas e alinhadas aos requisitos estabelecidos.

## 6. Etapas previstas

1. **Descoberta e visão do produto:** definição do problema, dos usuários, dos objetivos e dos limites da solução.
2. **Seleção e análise dos dados:** escolha da base pública, compreensão das variáveis, análise exploratória e verificação da adequação dos dados.
3. **Especificação de Machine Learning:** definição dos algoritmos candidatos, dos procedimentos de validação e das métricas.
4. **Engenharia de requisitos:** requisitos funcionais e não funcionais, casos de uso e critérios de aceitação.
5. **Arquitetura e especificações técnicas:** componentes, interfaces, contratos, estrutura do projeto e decisões tecnológicas.
6. **Planejamento do pipeline de LLM:** organização dos prompts, contexto, instruções, *skills*, eventuais agentes e mecanismos de verificação.
7. **Implementação incremental:** geração, integração, revisão e teste dos componentes.
8. **Validação do produto:** avaliação do modelo, testes funcionais, análise de qualidade e verificação dos requisitos.
9. **Documentação e publicação:** instruções de instalação, execução, configuração e utilização.
10. **Experimento de reprodutibilidade:** execução independente do pipeline e comparação dos resultados.

A sequência e o detalhamento serão refinados à medida que o projeto evoluir. Alterações relevantes deverão ser registradas e relacionadas aos artefatos afetados.

## 7. Organização do repositório

A estrutura inicial proposta é:

```text
.
├── README.md
├── docs/
│   ├── 01-discovery/
│   ├── 02-data/
│   ├── 03-machine-learning/
│   ├── 04-requirements/
│   ├── 05-architecture/
│   ├── 06-llm-pipeline/
│   ├── 07-testing/
│   └── 08-reproducibility/
├── prompts/
├── skills/
├── agents/
├── src/
├── tests/
├── experiments/
└── requirements.txt
```

A estrutura será ajustada conforme os componentes efetivamente adotados e os artefatos produzidos.

## 8. Princípios orientadores

- **Orientação ao problema de negócio:** a tecnologia deverá responder a uma necessidade definida, e não ser um fim em si mesma.
- **Qualidade verificável:** os resultados deverão atender a critérios de aceitação e evidências de teste.
- **Documentação como artefato de engenharia:** decisões relevantes deverão ser registradas e versionadas.
- **Rastreabilidade:** requisitos, especificações, prompts, código e testes deverão manter relações identificáveis.
- **Validação independente:** código e decisões gerados por LLMs deverão ser verificados.
- **Transparência experimental:** resultados, limitações, falhas e intervenções humanas deverão ser documentados.
- **Reprodutibilidade:** as instruções e condições necessárias para executar novamente o processo deverão ser preservadas.
- **Evolução controlada:** mudanças relevantes deverão permitir identificar seus impactos no produto e no pipeline.

## 9. Status do projeto

**Fase atual:** planejamento, definição da visão do produto e estruturação da documentação.

A seleção definitiva do problema e da base de dados, os requisitos do sistema e as decisões arquiteturais serão formalizados nas etapas iniciais.

## 10. Contexto acadêmico

Projeto desenvolvido no contexto do mestrado profissional em Inteligência Computacional Aplicada às Decisões Financeiras.

