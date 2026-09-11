# Análise e Validação de Requisitos

Esta etapa tem como objetivo verificar a qualidade dos requisitos
levantados e identificar possíveis inconsistências, ambiguidades,
lacunas ou conflitos antes da evolução do projeto.

A análise considera os seguintes critérios:

- Consistência
- Completude
- Clareza e ausência de ambiguidade
- Testabilidade
- Rastreabilidade

---

## 1. Requisito em análise

**ID do Requisito:** RF002 — Gerenciamento de Postagens  
**Versão:** 1.1  
**Responsável pela análise:** Analista de Sistemas

---

## 2. Checklist de Qualidade

### 2.1 Consistência / Conflitos

**Status:** OK

O requisito não apresenta conflitos identificados com os demais
requisitos ou regras de negócio definidos para o sistema.

---

### 2.2 Completude

**Status:** AJUSTADO

Durante a análise, foi identificada uma lacuna relacionada ao
comportamento do sistema durante a exclusão de uma postagem com
registros relacionados.

**Ação realizada:** A situação foi analisada e documentada na
regra de negócio correspondente.

---

### 2.3 Clareza / Ausência de Ambiguidade

**Status:** OK

O requisito descreve de forma objetiva as operações esperadas
para o gerenciamento de postagens, evitando termos subjetivos
ou interpretações diferentes sobre o comportamento esperado.

---

### 2.4 Testabilidade

**Status:** OK

As operações descritas no requisito podem ser verificadas por
meio de cenários objetivos de criação, consulta, alteração e
exclusão de postagens, considerando também as regras de
autorização definidas para cada operação.

---

### 2.5 Rastreabilidade

**Status:** OK

O requisito está relacionado às regras de negócio aplicáveis
ao gerenciamento de postagens e ao objetivo de negócio
correspondente.

**Rastreabilidade:**

```text
Objetivo de Negócio
        ↓
RF002 — Gerenciamento de Postagens
        ↓
RN002 — Validação de Título e Texto
RN003 — Vínculo Obrigatório com Tema
RN004 — Autorização para Alteração
```
