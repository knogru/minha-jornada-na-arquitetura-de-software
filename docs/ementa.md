# Ementa · Plano de Estudos

!!! success "Progresso geral"
    **0 / 30 aulas concluídas** · Ainda não iniciado

    `░░░░░░░░░░░░░░░░░░░░░░░░░░░░░` 0%

---

## Sobre o Curso

Este plano de estudos foi estruturado para formar a mentalidade de um arquiteto de software por meio do domínio de estilos arquiteturais, atributos de qualidade, modelagem orientada a domínios (DDD), gestão de concorrência de dados, isolamento tático, governança automatizada e estratégias evolutivas de migração — tudo de forma **agnóstica a linguagens e frameworks**.

| | |
| :--- | :--- |
| **Total de aulas** | 30 horas de imersão ativa |
| **Dinâmica** | ~35 min de leitura analítica + ~25 min de atividade prática |
| **Módulos** | 8 marcos evolutivos |

---

## Módulo 1 · Fundamentos, O Papel do Arquiteto e Atributos de Qualidade

*Foco na desconstrução da complexidade e mapeamento de direcionadores de negócio.*

| Aula | Tema | Referência | Status |
| :--: | :--- | :--- | :----: |
| 01 | Definição de Arquitetura e a Lei de Conway | *Software Architecture in Practice* — Bass, Clements, Kazman (Cap. 1 e 2) | 🔒 |
| 02 | Atributos de Qualidade (Requisitos Não-Funcionais) | Documentação ISO/IEC 25010 | 🔒 |
| 03 | Acoplamento, Coesão e Complexidade | *Out of the Tar Pit* — Ben Moseley & Peter Marks | 🔒 |

---

## Módulo 2 · Estilos e Padrões Arquiteturais Clássicos

*Estudo dos pilares históricos e estruturais que fundamentam a engenharia de sistemas.*

| Aula | Tema | Referência | Status |
| :--: | :--- | :--- | :----: |
| 04 | Estilos Estruturais Básicos (Pipes & Filters e Cliente-Servidor) | *An Introduction to Software Architecture* — Garlan & Shaw | 🔒 |
| 05 | O Padrão de Arquitetura em Camadas | *POSA Vol. 1* — Buschmann et al. (Cap. 2, Seção 2.2) | 🔒 |
| 06 | O Padrão Model-View-Controller (MVC) | *POSA Vol. 1* — Buschmann et al. (Cap. 2, Seção 2.4) | 🔒 |
| 07 | SOA (Service-Oriented Architecture) | *Software Design and Architecture Specialization* — University of Alberta | 🔒 |

---

## Módulo 3 · Padrões Modernos e Clean Architecture

*Isolamento tático do coração do negócio contra volatilidade tecnológica.*

| Aula | Tema | Referência | Status |
| :--: | :--- | :--- | :----: |
| 08 | Arquitetura Hexagonal (Ports and Adapters) | *Hexagonal Architecture* — Alistair Cockburn | 🔒 |
| 09 | Clean Architecture I — Limites Arquiteturais e Desacoplamento | *Clean Architecture* — Robert C. Martin (Cap. 15, 16 e 17) | 🔒 |
| 10 | Clean Architecture II — Regras de Negócio e Casos de Uso | *Clean Architecture* — Robert C. Martin (Cap. 19, 20 e 21) | 🔒 |
| 11 | Clean Architecture III — O Modelo dos Anéis Concêntricos | *Clean Architecture* — Robert C. Martin (Cap. 22) | 🔒 |
| 12 | Domain-Driven Design (Estratégico) | *DDD Distilled* — Vaughn Vernon (Cap. 1, 2 e 3) | 🔒 |
| 13 | Domain-Driven Design (Tático) | *DDD Distilled* — Vaughn Vernon (Cap. 4, 5 e 6) | 🔒 |

---

## Módulo 4 · Documentação e Representação Arquitetural

*Formas padronizadas de comunicar estruturas complexas para diferentes stakeholders.*

| Aula | Tema | Referência | Status |
| :--: | :--- | :--- | :----: |
| 14 | O Modelo 4+1 Visões e UML | *Architectural Blueprints — The "4+1" View Model* — Philippe Kruchten | 🔒 |
| 15 | O Modelo C4 (Modernização da Documentação) | *The C4 Model* — Simon Brown | 🔒 |

---

## Módulo 5 · Arquitetura de Dados, Concorrência e Padrões CQRS

*Tratamento de persistência, consistência e concorrência em sistemas distribuídos de alto rendimento.*

| Aula | Tema | Referência | Status |
| :--: | :--- | :--- | :----: |
| 16 | Teorema CAP e Bancos Isolados | *Brewer's Conjecture* — Seth Gilbert & Nancy Lynch | 🔒 |
| 17 | Transações ACID, Níveis de Isolamento e Locking | *Designing Data-Intensive Applications* — Martin Kleppmann (Cap. 7) | 🔒 |
| 18 | CQRS e Event Sourcing | Microsoft Patterns & Practices — CQRS Pattern e Event Sourcing Pattern | 🔒 |

---

## Módulo 6 · Sistemas Distribuídos e Escala Avançada

*Análise multidimensional da capacidade de carga e padrões de comunicação assíncrona.*

| Aula | Tema | Referência | Status |
| :--: | :--- | :--- | :----: |
| 19 | O Cubo de Escalabilidade I — Visão Geral e Eixo X | *The Art of Scalability* — Abbott & Fisher (Cap. 12) | 🔒 |
| 20 | O Cubo de Escalabilidade II — Eixo Y (Decomposição) | *The Art of Scalability* — Abbott & Fisher (Cap. 13) | 🔒 |
| 21 | O Cubo de Escalabilidade III — Eixo Z (Particionamento) | *The Art of Scalability* — Abbott & Fisher (Cap. 14) | 🔒 |
| 22 | Comunicação Assíncrona I — Estilos de Integração | *Enterprise Integration Patterns* — Hohpe & Woolf (Cap. 2) | 🔒 |
| 23 | Comunicação Assíncrona II — Canais de Mensageria | *Enterprise Integration Patterns* — Hohpe & Woolf (Cap. 3) | 🔒 |

---

## Módulo 7 · Avaliação e Evolução Arquitetural

*Governança sistêmica de código e validação de requisitos de estabilidade futuros.*

| Aula | Tema | Referência | Status |
| :--: | :--- | :--- | :----: |
| 24 | Avaliação Arquitetural e o Método ATAM | SEI Technical Report — *Evaluating Software Architectures using ATAM* | 🔒 |
| 25 | Arquiteturas Evolutivas I — O Conceito de Mutabilidade | *Building Evolutionary Architectures* — Ford, Parsons, Kua (Cap. 1) | 🔒 |
| 26 | Arquiteturas Evolutivas II — Projetando Fitness Functions | *Building Evolutionary Architectures* — Ford, Parsons, Kua (Cap. 2) | 🔒 |
| 27 | Arquiteturas Evolutivas III — Engenharia de Mudança Incremental | *Building Evolutionary Architectures* — Ford, Parsons, Kua (Cap. 3) | 🔒 |

---

## Módulo 8 · A Jornada de Refatoração e Desacoplamento

*Roteiros estruturados para modernização de sistemas legados e separação de bancos de dados.*

| Aula | Tema | Referência | Status |
| :--: | :--- | :--- | :----: |
| 28 | Estratégias de Migração I — Anatomia e Tipos de Monolito | *Monolith to Microservices* — Sam Newman (Cap. 1 e 2) | 🔒 |
| 29 | Estratégias de Migração II — O Padrão Strangler Fig | *Monolith to Microservices* — Sam Newman (Cap. 4) | 🔒 |
| 30 | Estratégias de Migração III — Decomposição de Bancos de Dados | *Monolith to Microservices* — Sam Newman (Cap. 5) | 🔒 |

---

!!! tip "Como atualizar o progresso"
    Ao concluir um fichamento, troque o ícone da aula de 🔒 para ✅ (ou ⏳ se estiver em andamento), atualize o contador no bloco de progresso no topo e faça o commit. O site atualiza automaticamente via GitHub Actions.