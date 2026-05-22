---
date: 2026-05-22
title: "Aula 08 · Arquitetura Hexagonal (Ports and Adapters)"
description: "Fichamento analítico sobre simetria arquitetural e o uso de abstrações para blindar o domínio de agentes externos."
authors:
  - aline
categories:
  - Módulo 3 · Padrões Modernos
tags:
  - hexagonal
  - ports-and-adapters
  - isolamento-de-domínio
reading_time: 8
aula: 8
modulo: 3
status: concluida   # concluida | em-andamento | pendente
---

---
# Aula 08 · Arquitetura Hexagonal (Ports and Adapters)

!!! info "Referência"
    **Obra:** Hexagonal Architecture  
    **Autor:** Alistair Cockburn  
    **Módulo:** 3 — Padrões Modernos e Clean Architecture  
    **Data da leitura:** 22/05/2026

---

## 1. Ideias-chave

### 1.1 [título da ideia]

Descrição da ideia com suas próprias palavras.

> "Citação exata do texto, se houver." — Cockburn, §3

**Síntese:** o que isso significa na prática, em suas palavras.

### 1.2 [título da ideia]

...

---

## 2. Análise crítica e conexões táticas

Sua análise pessoal sobre o conteúdo — concordâncias, tensões com outros conceitos, implicações práticas.

!!! tip "Conexão com aulas anteriores"
    Como este conceito se relaciona com o que foi visto antes — ex: a Lei de Conway (Aula 01) influencia diretamente onde as portas são desenhadas.

**Conexão com o projeto prático (M3 · Screaming E-Commerce Core):**  
Como o conceito se aplica ou aparece no mini projeto do módulo.

---

## 3. Atividade prática

**Enunciado:** Identificar as portas de entrada (Driving Ports), saídas (Driven Ports) e adaptadores para um caso de uso que processe notificações via SMS ou Email.

**Minha solução:**

```python
# seu pseudocódigo ou diagrama aqui
```

**Reflexão:** o que a atividade revelou ou confirmou sobre o conceito.

---

## 4. Vocabulário técnico

| Termo | Definição |
| :--- | :--- |
| **Driving Port** | Interface que representa uma intenção externa direcionada ao domínio |
| **Driven Port** | Interface que o domínio usa para se comunicar com o mundo externo |
| **Adaptador** | Implementação concreta de uma porta, conectando tecnologia ao domínio |

---

!!! quote "Para fixar"
    A frase, princípio ou imagem mental que você vai carregar desta aula.