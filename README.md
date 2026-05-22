Bem-vindo ao meu repositório central de estudos, fichamentos em **Arquitetura de Software**. Este espaço funciona como meu portfólio técnico, consolidando conceitos fundamentais de forma totalmente **agnóstica a linguagens, frameworks ou provedores de nuvem**.

O repositório foi estruturado utilizando a filosofia *Docs as Code*, onde toda a documentação teórica é escrita em Markdown, versionada via Git, integrada com diagramas vivos em Mermaid.js e publicada usando MkDocs.

---

## Estrutura do Repositório

*   `/docs`: Contém os fichamentos analíticos detalhados de cada aula, divididos por módulos.
*   `/projects`: Mini projetos conceituais ("mecanismos táticos") construídos sem dependências externas para provar os conceitos estudados.
*   `ementa.md`: O cronograma mestre de 30 aulas que guia esta jornada de aprendizado.

---

## Currículo e Módulos de Estudo

O plano de estudos está dividido em 8 grandes marcos evolutivos:

1. **Fundamentos e Atributos de Qualidade:** Alinhamento de trade-offs de negócio, Lei de Conway e desconstrução da complexidade essencial vs. acidental.
2. **Estilos Arquiteturais Clássicos:** Do modelo em camadas fechadas (*Jail Layers*) ao MVC estrutural e barramentos corporativos (SOA).
3. **Padrões Modernos e Clean Architecture:** Domínio do isolamento tático (*Ports & Adapters*) e os pilares estratégicos/táticos do Domain-Driven Design (DDD).
4. **Documentação e Representação:** Comunicação técnica eficaz utilizando o Modelo 4+1 visões e o Modelo C4 (Abstração hierárquica).
5. **Arquitetura de Dados e Concorrência:** Teorema CAP, níveis de isolamento transacional, travas de concorrência e segregação de leitura/escrita (CQRS/Event Sourcing).
6. **Sistemas Distribuídos e Escala:** Engenharia de alta carga baseada no *AKF Scale Cube* (Eixos X, Y e Z) e padrões de integração assíncrona.
7. **Avaliação e Evolução:** Governança contínua através de *Architecture Fitness Functions* e aplicação do método ATAM.
8. **Jornada de Refatoração:** Padrões de estrangulamento (*Strangler Fig*) e técnicas para decomposição de bancos de dados legados compartilhados.

---

## Portfólio de Mini Projetos

Cada módulo é acompanhado por um artefato prático construído sob a premissa de **zero frameworks pesados**:

*   **M1: Core Logger & Sanitizer** — Engine pura de captura de auditoria aplicando inversão de dependência absoluta.
*   **M2: Pipes & Filters Pipeline** — Motor CLI de processamento de streams de dados baseado em filtros intercambiáveis.
*   **M3: The Screaming E-Commerce Core** — Camada de domínio Clean Architecture onde as pastas gritam o modelo de negócio, isoladas de I/O.
*   **M4: Architecture Living Blueprint** — Documentação viva dos níveis 1 e 2 do C4 mapeada inteiramente via código (*Mermaid.js*).
*   **M5: In-Memory Event Store** — Motor de projeção CQRS assíncrono com controle de versão e concorrência otimista manual.
*   **M6: AKF Scale Cube Router** — Gateway conceitual demonstrando roteamento dinâmico e isolamento horizontal para o Eixo Z (*Sharding*).
*   **M7: Architectural Fitness Gate** — Script automatizado de análise estática para CI que reprova o build caso haja violação de limites de acoplamento.
*   **M8: Migration RFC Blueprint** — Artigo técnico e especificação de engenharia detalhando a estratégia de decomposição de um banco de dados legado.

---

## 🚀 Como Rodar e Visualizar Este Repositório Localmente

Toda a documentação é compilada em um site estático. Para rodar a documentação na sua máquina:

1. Certifique-se de ter o Python instalado.
2. Instale o MkDocs e o tema de preferência (ex: Material):
   
```bash
   pip install mkdocs-material