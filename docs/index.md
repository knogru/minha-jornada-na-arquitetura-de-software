# Minha Jornada em Arquitetura de Software

Bem-vindo ao meu repositório central de estudos e fichamentos em Arquitetura de Software — um portfólio técnico construído de forma **agnóstica a linguagens, frameworks e provedores de nuvem**.

---

## Sobre este espaço

Este repositório segue a filosofia *Docs as Code*: toda documentação teórica é escrita em Markdown, versionada via Git, ilustrada com diagramas vivos em Mermaid.js e publicada com MkDocs.

O objetivo não é acumular anotações — é **construir entendimento progressivo**, do fundamento ao trade-off real, módulo por módulo.

---

## Estrutura

| Diretório | Conteúdo |
|---|---|
| `/docs` | Fichamentos analíticos por módulo |
| `/projects` | Mini projetos conceituais sem frameworks pesados |
| `ementa.md` | Cronograma mestre das 30 aulas |

---

## Módulos de Estudo

A jornada está dividida em **8 marcos evolutivos**:

| # | Marco | Foco principal |
|---|---|---|
| 1 | Fundamentos e Qualidade | Trade-offs, Lei de Conway, complexidade essencial vs. acidental |
| 2 | Estilos Clássicos | Camadas fechadas, MVC estrutural, SOA |
| 3 | Clean Architecture e DDD | Ports & Adapters, tática e estratégia do Domain-Driven Design |
| 4 | Documentação e Representação | Modelo 4+1, Modelo C4 |
| 5 | Dados e Concorrência | Teorema CAP, isolamento transacional, CQRS/Event Sourcing |
| 6 | Sistemas Distribuídos | AKF Scale Cube, integração assíncrona |
| 7 | Avaliação e Evolução | Architecture Fitness Functions, método ATAM |
| 8 | Refatoração Legada | Strangler Fig, decomposição de bancos compartilhados |


!!! tip "Onde estou agora"
    **Módulo 1 · Fundamentos, O Papel do Arquiteto e Atributos de Qualidade**  
    Aula atual: [01 · Definição de Arquitetura e a Lei de Conway](blog/posts/modulo-1-aula-01-definicao-de-arquitetura-e-lei-de-conway.md)  
    [Ver ementa completa →](ementa.md)


---

## Portfólio de Mini Projetos

Cada módulo tem um artefato prático construído sob a premissa de **zero frameworks pesados**:

| Projeto | Descrição |
|---|---|
| **M1 · Core Logger & Sanitizer** | Engine de auditoria com inversão de dependência absoluta |
| **M2 · Pipes & Filters Pipeline** | Motor CLI de streams com filtros intercambiáveis |
| **M3 · Screaming E-Commerce Core** | Domínio Clean Architecture onde as pastas gritam o negócio |
| **M4 · Architecture Living Blueprint** | Níveis 1 e 2 do C4 mapeados inteiramente em Mermaid.js |
| **M5 · In-Memory Event Store** | Projeção CQRS assíncrona com concorrência otimista manual |
| **M6 · AKF Scale Cube Router** | Gateway conceitual com roteamento dinâmico e sharding (Eixo Z) |
| **M7 · Architectural Fitness Gate** | Script de CI que reprova o build em violações de acoplamento |
| **M8 · Migration RFC Blueprint** | Especificação técnica de decomposição de banco de dados legado |

---

!!! tip "Por onde começar?"
    Acesse a [Ementa](ementa.md) para ver o cronograma completo, ou navegue pelos módulos no menu lateral.