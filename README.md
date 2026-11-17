# Vreamshaper — MVP de Gestão Solidária

Repositório oficial do Minimum Viable Product (MVP) desenvolvido para a **Associação Comunitária Mãos Solidárias**, localizada no Jardim São Luís (São Paulo). O sistema foi projetado para otimizar a triagem de famílias vulneráveis, eliminar entregas duplicadas mensais e gerenciar o estoque de perecíveis sob a lógica FEFO (*First Expire, First Out*), operando em modo *Offline-First*.

## 🚀 Pilha Tecnológica
* **Frontend:** Angular (PWA) + TypeScript + Angular Material
* **Persistência Local:** Dexie.js + IndexedDB (suporte offline integral)
* **Backend e Banco de Dados Remoto:** Supabase (PostgreSQL 15+ com Row Level Security)
* **Hospedagem:** Vercel / Netlify (CDN Global)

## 📱 Funcionalidades Principais (Requisitos Funcionais)
* **RF-01 e RF-02:** Cadastro de núcleos familiares e busca rápida otimizada por CPF.
* **RF-03:** Trava automática de segurança impedindo retirada duplicada em um intervalo de 30 dias.
* **RF-04 e RF-05:** Gestão de lotes de alimentos com ordenação FEFO e alertas preventivos de vencimento em 15 dias.
* **RF-06:** Painel consolidado de indicadores operacionais.

## 🔒 Segurança e Acessibilidade (RNF-01 a RNF-04)
* Autenticação via Supabase Auth e controle de acesso baseado em políticas RLS no PostgreSQL.
* Conformidade com diretrizes OWASP Top 10 e sanitização de dados no Angular.
* Design *Mobile-First* com alvos de toque $\ge 44 \times 44\text{ px}$, contraste $\ge 4,5:1$ e alertas multimodais (cor + ícone + texto) acessíveis em conformidade com a WCAG 2.1 AA.

## 🛠️
