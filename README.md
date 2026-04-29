# ⚖️ Claus.io

> Plataforma de análise inteligente de documentos jurídicos — desenvolvida na Universidade Católica de Brasília.

---

## 📌 Sobre o projeto

O **Claus.io** é uma plataforma baseada em inteligência artificial capaz de processar e analisar documentos jurídicos extensos. A solução permite o upload de arquivos nos formatos **TXT** e **DOCX**, gerando automaticamente resumos executivos em linguagem clara e identificando riscos jurídicos classificados por nível de criticidade (alto, médio e baixo).

O projeto visa reduzir o tempo de análise documental, aumentar a produtividade de equipes jurídicas e apoiar a tomada de decisão com maior agilidade e assertividade — tanto em escritórios de advocacia quanto em órgãos públicos.

---

## 🚀 Funcionalidades

| Funcionalidade | Prioridade |
|---|---|
| Upload de documentos (TXT e DOCX) | Crítico |
| Processamento via API com prompt jurídico especializado | Crítico |
| Geração automática de resumo executivo | Crítico |
| Identificação e classificação de riscos (alto / médio / baixo) | Crítico |
| Destaque visual dos riscos por cores | Útil |
| Personalização por nicho jurídico (cível, trabalhista, criminal...) | Importante |

---

## 👥 Perfis de Usuário

- **Usuário Externo (Advogado / Analista / Servidor)** — realiza upload de documentos, analisa resumos e avalia riscos identificados.
- **Administrador (Usuário Interno)** — personaliza o comportamento da plataforma conforme o nicho jurídico de atuação.

---

## 🏗️ Arquitetura

A stack definida para o MVP é composta por:

```
┌─────────────┐     ┌───────────────────────────────┐
│    NGINX     │◄───►│  Frontend  │  Backend  │  DB  │
│ (proxy rev.) │     │   React    │  Node.js  │  PG  │
└─────────────┘     └───────────────────────────────┘
       │
       ▼
  Cloud / API de IA (Anthropic / OpenAI)
```

- **Frontend**: React (interface dinâmica e responsiva)
- **Backend**: Node.js (lógica de negócio + integração com API de IA)
- **Banco de dados**: PostgreSQL (armazenamento seguro de registros e metadados)
- **Proxy reverso**: NGINX (roteamento e segurança das requisições)
- **Infraestrutura**: Cloud (escalabilidade conforme demanda)

---

## 📋 Requisitos Não-Funcionais

- Acessível via navegadores modernos, sem instalação local
- Interface simples e intuitiva para usuários com qualquer nível técnico
- Hospedagem em nuvem com suporte à escalabilidade
- Conformidade com normas de tratamento de dados (LGPD e contexto jurídico)
- Disponibilidade e consistência nos resultados gerados

---

## 💰 Estimativa de Custo

| Item | Valor estimado |
|---|---|
| Desenvolvimento do MVP | R$ 15.000 – R$ 60.000 |
| Custo recorrente mensal (API de IA + hospedagem) | R$ 500 – R$ 3.000/mês |

---

## 📁 Documentação

| Documento | Versão | Data |
|---|---|---|
| Documento de Visão | 1.2 | 01/04/2026 |

A documentação completa do projeto está disponível na pasta `/docs`.

---

## 👩‍💻 Autores

| Nome | E-mail | Papel |
|---|---|---|
| Nicole Flaminio | nicole.flaminio@a.ucb.br | Coautora |
| Matheus Neiva | matheus.neiva@a.ucb.br | Coautor |
| Paulo Gustavo | paulo.gmartins@a.ucb.br | Coautor |

---

## 🏫 Instituição

Desenvolvido como projeto acadêmico na **Universidade Católica de Brasília (UCB)**
QS 07 – Lote 01 – EPCT, Taguatinga, Brasília — [ucb.catolica.edu.br](https://ucb.catolica.edu.br)

---

*Versão do README: 1.0 — Abril/2026*
