Este documento apresenta o plano de estudos estruturado para o domínio conceitual e prático de **Arquitetura de Software**. O currículo foi desenvolvido cruzando as diretrizes acadêmicas de universidades de referência (UFC, UPE, IFRN), programas internacionais (Coursera/University of Alberta) e os padrões práticos de desenvolvimento de sistemas enterprise.

## Objetivo do Curso
Formar a mentalidade de um arquiteto de software por meio do domínio de estilos arquiteturais, atributos de qualidade, modelagem orientada a domínios (DDD), gestão de concorrência de dados, isolamento tático, governança automatizada e estratégias evolutivas de migração. Tudo isso de forma **agnóstica a linguagens e frameworks**.

## Estrutura de Carga Horária
* **Total:** 30 aulas (30 horas de imersão ativa)
* **Dinâmica por Aula:** ~35 minutos de leitura/estudo analítico + ~25 minutos de resolução de atividade teórica ou prática individual.

---

## Cronograma Detalhado das Aulas

### Módulo 1: Fundamentos, O Papel do Arquiteto e Atributos de Qualidade
*Foco na desconstrução da complexidade e mapeamento de direcionadores de negócio.*

#### Aula 01: Definição de Arquitetura e a Lei de Conway
*   **Objetivo:** Compreender que arquitetura reside nas decisões difíceis de mudar e como as estruturas organizacionais moldam os sistemas.
*   **Material de Apoio:** *Software Architecture in Practice* (Bass, Clements, Kazman) — Capítulos 1 e 2.
*   **Atividade Prática:** Analisar um sistema real de larga escala (ex: WhatsApp, iFood) e mapear 3 decisões estruturais de alto impacto baseadas em trade-offs de negócio.

#### Aula 02: Atributos de Qualidade (Requisitos Não-Funcionais)
*   **Objetivo:** Explorar os pilares da norma ISO/IEC 25010 e entender o conflito nativo entre diferentes direcionadores de qualidade.
*   **Material de Apoio:** Documentação técnica da norma ISO/IEC 25010 (Seções de Qualidade de Produto).
*   **Atividade Prática:** Escolher três cenários de atributos conflitantes (ex: Segurança vs. Desempenho) e redigir uma matriz de priorização justificando decisões para um sistema bancário vs. um portal de notícias.

#### Aula 03: Acoplamento, Coesão e Complexidade
*   **Objetivo:** Distinguir Complexidade Essencial de Complexidade Acidental e estudar os limites do acoplamento de código.
*   **Material de Apoio:** Paper Acadêmico Clássico: *Out of the Tar Pit* (Ben Moseley & Peter Marks).
*   **Atividade Prática:** Escrever em pseudocódigo duas estruturas de componentes altamente acopladas e refatorá-las aplicando inversão de dependência para isolar a política da mecânica de IO.

---

### Módulo 2: Estilos e Padrões Arquiteturais Clássicos
*Estudo dos pilares históricos e estruturais que fundamentam a engenharia de sistemas.*

#### Aula 04: Estilos Estruturais Básicos (Pipes & Filters e Cliente-Servidor)
*   **Objetivo:** Analisar como o fluxo de dados determina a topologia de um sistema e as origens da computação distribuída.
*   **Material de Apoio:** Artigo clássico: *An Introduction to Software Architecture* (David Garlan & Mary Shaw).
*   **Atividade Prática:** Desenhar um fluxograma arquitetural usando o modelo Pipes & Filters para um motor agnóstico de processamento e sanitização de logs textuais.

#### Aula 05: O Padrão de Arquitetura em Camadas (Layers)
*   **Objetivo:** Dominar o isolamento vertical de responsabilidades, regras de visibilidade estrita (Jail Layers) e o princípio da transparência de localização.
*   **Material de Apoio:** *Pattern-Oriented Software Architecture (POSA) - Vol 1* (Buschmann et al.) — Capítulo 2, Seção 2.2 ("Layers").
*   **Atividade Prática:** Estruturar conceitualmente a árvore de componentes de um sistema que obedeça rigidamente ao padrão de camadas fechadas, impedindo vazamento de escopo.

#### Aula 06: O Padrão Model-View-Controller (MVC)
*   **Objetivo:** Estudar os mecanismos de desacoplamento entre a exibição, o controle de fluxo e o modelo central de dados.
*   **Material de Apoio:** *Pattern-Oriented Software Architecture (POSA) - Vol 1* (Buschmann et al.) — Capítulo 2, Seção 2.4 ("Model-View-Controller").
*   **Atividade Prática:** Construir um diagrama de sequência abstrato mapeando a troca de mensagens e notificações assíncronas entre as três entidades do MVC durante uma atualização de estado.

#### Aula 07: SOA (Service-Oriented Architecture)
*   **Objetivo:** Compreender a integração empresarial baseada em serviços independentes, Enterprise Service Bus (ESB) e governança de contratos.
*   **Material de Apoio:** Módulo de Arquitetura SOA do programa *Software Design and Architecture Specialization* (University of Alberta).
*   **Atividade Prática:** Redigir a especificação de um contrato de interface pública (estilo contrato agnóstico WSDL/YAML) para um subsistema de contabilidade corporativo.

---

### Módulo 3: Padrões Modernos e Clean Architecture (Foco em Domínio)
*Isolamento tático do coração do negócio contra volatilidade tecnológica.*

#### Aula 08: Arquitetura Hexagonal (Ports and Adapters)
*   **Objetivo:** Compreender o conceito de simetria arquitetural e o uso de abstrações para blindar o domínio de agentes externos.
*   **Material de Apoio:** Artigo original: *Hexagonal Architecture* (Alistair Cockburn).
*   **Atividade Prática:** Identificar as portas de entrada (Driving Ports), saídas (Driven Ports) e adaptadores para um caso de uso que processe notificações via SMS ou Email.

#### Aula 09: Clean Architecture I — Limites Arquiteturais e Desacoplamento
*   **Objetivo:** Estudar o desenho de fronteiras de software, custos de abstração e os princípios de independência de desenvolvimento.
*   **Material de Apoio:** *Clean Architecture* (Robert C. Martin) — Capítulos 15, 16 e 17.
*   **Atividade Prática:** Redigir uma análise técnica de uma página defendendo como limites mal posicionados transformam um projeto promissor em um "monolito emaranhado".

#### Aula 10: Clean Architecture II — Regras de Negócio e Casos de Uso
*   **Objetivo:** Isolar e mapear políticas de alto nível (Entidades) de lógicas focadas na aplicação (Casos de Uso), aplicando a Screaming Architecture.
*   **Material de Apoio:** *Clean Architecture* (Robert C. Martin) — Capítulos 19, 20 e 21.
*   **Atividade Prática:** Modelar o esqueleto textual de um Caso de Uso de "Cancelamento de Assinatura", separando o que é validação da regra de negócio da mecânica de execução do fluxo.

#### Aula 11: Clean Architecture III — O Modelo dos Anéis Concêntricos
*   **Objetivo:** Aplicar de maneira absoluta a Regra da Dependência e os mecanismos de inversão de controle para cruzar limites arquiteturais.
*   **Material de Apoio:** *Clean Architecture* (Robert C. Martin) — Capítulo 22.
*   **Atividade Prática:** Desenhar o grafo de dependências estruturais demonstrando como um componente de persistência de dados obedece às diretrizes do núcleo sem que este conheça sua existência.

#### Aula 12: Domain-Driven Design (Estratégico)
*   **Objetivo:** Aprender a mapear a complexidade corporativa por meio de Bounded Contexts, Context Maps e o desenvolvimento de uma Linguagem Ubíqua.
*   **Material de Apoio:** *Domain-Driven Design Distilled* (Vaughn Vernon) — Capítulos 1, 2 e 3.
*   **Atividade Prática:** Desenhar o mapa de contextos para uma aplicação de streaming de vídeo, delimitando as fronteiras de "Identidade", "Catálogo" e "Faturamento".

#### Aula 13: Domain-Driven Design (Tático)
*   **Objetivo:** Dominar os blocos de construção internos do domínio: Entidades com ciclo de vida, Value Objects imutáveis, Repositories e raízes de Agregados.
*   **Material de Apoio:** *Domain-Driven Design Distilled* (Vaughn Vernon) — Capítulos 4, 5 e 6.
*   **Atividade Prática:** Desenhar ou codificar conceitualmente em pseudocódigo um Agregado de "Pedido", definindo regras invariantes que protejam a consistência de seus itens internos.

---

### Módulo 4: Documentação e Representação Arquitetural
*Formas padronizadas de comunicar estruturas complexas para diferentes stakeholders.*

#### Aula 14: O Modelo 4+1 Visões e UML
*   **Objetivo:** Compreender as visões Lógica, de Processo, de Desenvolvimento, Física e de Cenários para mitigar ambiguidades em projetos.
*   **Material de Apoio:** Paper original: *Architectural Blueprints — The "4+1" View Model of Software Architecture* (Philippe Kruchten).
*   **Atividade Prática:** Elaborar um Diagrama de Implantação estruturado (UML - Visão Física) descrevendo a topologia de servidores e roteadores de uma aplicação de alta disponibilidade.

#### Aula 15: O Modelo C4 (Modernização da Documentação)
*   **Objetivo:** Dominar a abstração hierárquica (Mapas do Sistema) dividida em Contexto, Containers, Componentes e Código.
*   **Material de Apoio:** Guia oficial de especificação e exemplos do *The C4 Model* (Simon Brown).
*   **Atividade Prática:** Utilizar a abordagem "Diagramas como Código" (Mermaid.js ou Structurizr) para documentar o Nível 1 (Contexto) e o Nível 2 (Containers) do projeto em estudo.

---

### Módulo 5: Arquitetura de Dados, Concorrência e Padrões CQRS
*Tratamento de persistência, consistência e concorrência em sistemas distribuídos de alto rendimento.*

#### Aula 16: Teorema CAP e Bancos Isolados
*   **Objetivo:** Compreender os limites de consistência, disponibilidade e tolerância a partições, e estudar o impacto do isolamento de dados por serviço.
*   **Material de Apoio:** Paper de pesquisa original: *Brewer's Conjecture and the Feasibility of Consistent, Available, Partition-Tolerant Web Services* (Seth Gilbert & Nancy Lynch).
*   **Atividade Prática:** Formular um parecer de arquitetura justificando a escolha entre um desenho CP (Consistente/Particionado) vs. AP (Disponível/Particionado) para um sistema de controle de inventário.

#### Aula 17: Transações ACID, Níveis de Isolamento e Locking
*   **Objetivo:** Dominar os mecanismos internos de motores de banco de dados (Read Committed, Serializable) e as estratégias de travas de concorrência.
*   **Material de Apoio:** *Designing Data-Intensive Applications* (Martin Kleppmann) — Capítulo 7 ("Transactions").
*   **Atividade Prática:** Escrever um roteiro passo a passo demonstrando graficamente como evitar o problema da atualização perdida (*lost update*) utilizando o padrão Optimistic Locking com controle de versão.

#### Aula 18: CQRS e Event Sourcing
*   **Objetivo:** Separar caminhos de leitura e escrita para otimização de performance e estudar o armazenamento de estados como uma série de eventos imutáveis.
*   **Material de Apoio:** Documentação arquitetural Microsoft Patterns & Practices (Seções: *CQRS Pattern* e *Event Sourcing Pattern*).
*   **Atividade Prática:** Desenhar o fluxo de dados de uma transação que grava comandos em uma base relacional normalizada e atualiza uma base NoSQL otimizada para consultas através de projeções de eventos.

---

### Módulo 6: Sistemas Distribuídos e Escala Avançada
*Análise multidimensional da capacidade de carga e padrões de comunicação assíncrona.*

#### Aula 19: O Cubo de Escalabilidade I — Visão Geral e Eixo X
*   **Objetivo:** Estudar o modelo AKF Scale Cube e o particionamento via replicação horizontal de poder computacional sem estado compartilhado.
*   **Material de Apoio:** *The Art of Scalability* (Martin Abbott & Michael Fisher) — Capítulo 12.
*   **Atividade Prática:** Provar analiticamente as falhas de escalabilidade horizontal do Eixo X se a camada de dados centralizada se mantiver sob acoplamento temporal estreito.

#### Aula 20: O Cubo de Escalabilidade II — O Eixo Y (Decomposição)
*   **Objetivo:** Aprender a decompor grandes ecossistemas em partes menores através de especialização funcional e separação de substantivos/verbos de negócio.
*   **Material de Apoio:** *The Art of Scalability* (Martin Abbott & Michael Fisher) — Capítulo 13.
*   **Atividade Prática:** Tomar um sistema monolítico financeiro massivo e desenhar uma proposta de quebra baseada no Eixo Y justificando os novos limites.

#### Aula 21: O Cubo de Escalabilidade III — O Eixo Z (Particionamento de Dados)
*   **Objetivo:** Estudar as técnicas de sharding de bancos de dados, chaves de roteamento e distribuição geográfica de dados por perfil de cliente.
*   **Material de Apoio:** *The Art of Scalability* (Martin Abbott & Michael Fisher) — Capítulo 14.
*   **Atividade Prática:** Criar a especificação conceitual de um algoritmo de roteamento de conexões que direcione requisições para partições de banco isoladas com base no identificador único do locatário (*Tenant ID*).

#### Aula 22: Comunicação Assíncrona I — Estilos de Integração de Sistemas
*   **Objetivo:** Analisar criticamente as abordagens de transferência de arquivos, bancos de dados compartilhados, RPC e mensageria distribuída.
*   **Material de Apoio:** *Enterprise Integration Patterns (EIP)* (Gregor Hohpe & Bobby Woolf) — Capítulo 2 ("Integration Styles").
*   **Atividade Prática:** Construir uma tabela comparativa avaliando os 4 estilos com base em Latência, Acoplamento Temporal, Confiabilidade e Facilidade de Mudança.

#### Aula 23: Comunicação Assíncrona II — Canais de Mensageria Básicos
*   **Objetivo:** Dominar a semântica de entrega e o comportamento dos canais do tipo Ponto a Ponto (*Message Queue*) e Publicador-Assinante (*Publish-Subscribe*).
*   **Material de Apoio:** *Enterprise Integration Patterns (EIP)* (Gregor Hohpe & Bobby Woolf) — Capítulo 3 (Seções: *Point-to-Point Channel* e *Publish-Subscribe Channel*).
*   **Atividade Prática:** Mapear o ciclo de vida das mensagens de uma plataforma de entrega, indicando em qual etapa se deve usar um canal exclusivo vs. um canal de difusão de eventos.

---

### Módulo 7: Avaliação e Evolução Arquitetural
*Governança sistêmica de código e validação de requisitos de estabilidade futuros.*

#### Aula 24: Avaliação Arquitetural e o Método ATAM
*   **Objetivo:** Compreender a aplicação prática do Architecture Tradeoff Analysis Method para validar decisões antes da implementação em larga escala.
*   **Material de Apoio:** Technical Report do Software Engineering Institute (SEI): *Evaluating Software Architectures using ATAM*.
*   **Atividade Prática:** Construir uma Árvore de Utilidade (Utility Tree) focada no atributo de Disponibilidade, definindo cenários reais de estímulo, ambiente e resposta esperada do sistema.

#### Aula 25: Arquiteturas Evolutivas I — O Conceito de Mutabilidade
*   **Objetivo:** Entender o ciclo de degradação arquitetural e as regras para projetar softwares preparados para mudanças previsíveis e imprevisíveis.
*   **Material de Apoio:** *Building Evolutionary Architectures* (Neal Ford, Rebecca Parsons, Patrick Kua) — Capítulo 1.
*   **Atividade Prática:** Escrever uma dissertação analítica avaliando criticamente os custos ocultos do planejamento excessivo inicial (*Upfront Architecture*) face à evolução ágil do mercado.

#### Aula 26: Arquiteturas Evolutivas II — Projetando Fitness Functions
*   **Objetivo:** Conceituar funções de fitness contínuas e automatizadas para validar a integridade estrutural diretamente nas esteiras de automação.
*   **Material de Apoio:** *Building Evolutionary Architectures* (Neal Ford et al.) — Capítulo 2.
*   **Atividade Prática:** Estruturar em pseudocódigo lógico a validação de uma regra de conformidade que impeça que pacotes do domínio importem diretamente bibliotecas de infraestrutura.

#### Aula 27: Arquiteturas Evolutivas III — Engenharia de Mudança Incremental
*   **Objetivo:** Mitigar riscos de regressão operacional de arquitetura no ecossistema de produção usando esteiras de deploy estruturadas.
*   **Material de Apoio:** *Building Evolutionary Architectures* (Neal Ford et al.) — Capítulo 3.
*   **Atividade Prática:** Desenhar o fluxo lógico de uma esteira de CI/CD agnóstica que contenha gatilhos para reprovar um build baseado em índices de acoplamento aferidos via análise estática.

---

### Módulo 8: A Jornada de Refatoração e Desacoplamento
*Roteiros estruturados para modernização de sistemas legados e separação de bancos de dados.*

#### Aula 28: Estratégias de Migração I — Anatomia e Tipos de Monolito
*   **Objetivo:** Avaliar os gatilhos corretos para desmembramento de sistemas centrais e entender diferentes anatomias monolíticas.
*   **Material de Apoio:** *Monolith to Microservices* (Sam Newman) — Capítulos 1 e 2.
*   **Atividade Prática:** Elaborar um checklist organizacional e técnico com 5 critérios de corte fundamentais que justifiquem a quebra de um sistema integrado para microsserviços.

#### Aula 29: Estratégias de Migração II — O Padrão Strangler Fig
*   **Objetivo:** Dominar o ciclo de interceptação, coexistência e substituição gradativa de sistemas antigos sem interrupção de serviços.
*   **Material de Apoio:** *Monolith to Microservices* (Sam Newman) — Capítulo 4 (Seção: *Strangler Fig Pattern*).
*   **Atividade Prática:** Desenhar em 3 estágios (Início, Transição e Conclusão) a arquitetura de migração de uma rota legada utilizando um proxy reverso para estrangulamento da funcionalidade antiga.

#### Aula 30: Estratégias de Migração III — Decomposição de Bancos de Dados
*   **Objetivo:** Estudar o desacoplamento de tabelas compartilhadas vivos e o uso de sincronização assíncrona baseada em Change Data Capture (CDC).
*   **Material de Apoio:** *Monolith to Microservices* (Sam Newman) — Capítulo 5 ("Decomposing the Database").
*   **Atividade Prática:** Projetar a estratégia passo a passo de quebra de uma tabela altamente compartilhada de "Transações", detalhando o período de dupla escrita em produção e reconciliação sem perdas.