<div align="center">

<img src="https://capsule-render.vercel.app/api?type=soft&color=gradient&customColorList=2&height=200&section=header&text=🏛️%20RecentroConecta&fontSize=48&fontColor=fff&animation=fadeIn&desc=Transformação%20Digital%20•%20Parque%20Francisco%20Brennand%20•%20Recife&descSize=16&descAlignY=74" width="100%"/>

<br/>

[![Status](https://img.shields.io/badge/Status-MVP%20em%20produção-brightgreen?style=for-the-badge)]()
[![Cesar School](https://img.shields.io/badge/Cesar%20School-GTI%203º%20Período-0057B7?style=for-the-badge)]()
[![Cliente](https://img.shields.io/badge/Cliente-Prefeitura%20do%20Recife-E63946?style=for-the-badge)]()
[![Validação](https://img.shields.io/badge/MVP-95%25%20validado-00B4D8?style=for-the-badge)]()

**🔗 MVP em produção:** [v0-recentro-conecta-prototype.vercel.app](https://v0-recentro-conecta-prototype.vercel.app/)

</div>

---

## 🎯 Sobre o Projeto

**RecentroConecta** é uma solução de transformação digital para o **Recentro (Prefeitura do Recife)** e o **Parque de Esculturas Francisco Brennand**. O projeto substituiu processos manuais por uma plataforma digital integrada.

Desenvolvido no **Cesar School** como projeto real com cliente real — da imersão no campo até o MVP em produção, em 6 sprints.

---

## 🚀 Funcionalidades Entregues

| Módulo | Descrição |
|---|---|
| 🎫 **Bilheteria Digital** | Compra e emissão de ingressos online |
| 📅 **Agendamento de Grupos** | Reserva de visitas com gestão de parceiros |
| 📱 **QR Codes Interativos** | Conteúdo multimídia vinculado às esculturas |
| 📊 **Dashboard Operacional** | Painel em tempo real: visitas e engajamento |
| 🔒 **Gestão de Funcionários** | Administradores e operadores |

---

## 🏗️ Arquitetura do Sistema

```
[Visitante / Administrador]
          ↓
  [Frontend — Next.js]
  [Deploy: Vercel (Serverless)]
          ↓ REST API
  [Backend — Supabase]
  ├── PostgreSQL         → banco relacional
  ├── Row-Level Security → segurança por perfil
  ├── Auth              → autenticação
  ├── Storage           → mídias dos QR Codes
  └── Realtime          → dashboard ao vivo
```

---

## 🗄️ Modelo de Dados

Banco em **PostgreSQL via Supabase** com 8 entidades:

| Entidade | Propósito | FK |
|---|---|---|
| **Esculturas** | Conteúdo interativo + QR Code | — |
| **Ingressos** | Controle de acesso | — |
| **Agendamentos** | Visitas em grupo | — |
| **Visitantes_Agendados** | Detalhe por grupo | → Agendamentos |
| **Visitas_Esculturas** | Engajamento via QR | → Ingressos + Esculturas |
| **Funcionários** | Administradores | — |
| **Parceiros** | Escolas, hotéis | — |
| **Feedback** | Satisfação para dashboard | → Ingressos |
| **Status_Operacional** | Status em tempo real | — |

---

## 📋 Artefatos de UX & Produto

- ✅ Imersão com o cliente — observação presencial no parque
- ✅ Mapa de Empatia e Persona (visitante e grupos escolares)
- ✅ Jornada do Usuário e Service Blueprint
- ✅ UX/UI Design — prototipagem e testes aprovados
- ✅ Modelagem do BD (PostgreSQL/Supabase — SR2)
- ✅ Especificação de Requisitos funcionais e não funcionais
- ✅ Scripts SQL: DDL, DML e DQL completos

---

## 👩‍💻 Contribuição da Beatriz

- 🔍 Imersão com o cliente — pesquisa de campo no parque
- 🎨 Design de UX/UI — prototipagem e testes
- 🗺️ Service Blueprint e Jornada do Usuário
- 👤 Definição de Persona
- 🗄️ Apoio na modelagem do banco de dados relacional
- 📝 Especificação de requisitos
- 🔄 Gestão ágil com Scrum — 6 sprints, retrospectivas Sailboat

---

## 🛠️ Stack Tecnológica

![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)

---

## 📊 Resultados

| Métrica | Resultado |
|---|---|
| ✅ Requisitos validados | **95%** |
| 🔄 Sprints concluídos | **6** |
| 🚀 Ambiente | **Produção (Vercel + Supabase)** |
| 🧪 Testes de usabilidade | **Aprovados** |
| 🗄️ Entidades no banco | **8 tabelas relacionais** |

---

## 🔗 Links

- **MVP:** [v0-recentro-conecta-prototype.vercel.app](https://v0-recentro-conecta-prototype.vercel.app/)
- **Cliente:** [Recentro — Prefeitura do Recife](https://www2.recife.pe.gov.br/)

---

## 👥 Equipe

Cesar School — GTI 3º Período (2025):
Aynoã Gomes · **Beatriz Amaral** · Cauã · Danilo Brito · Gilvanira · Leônidas · Marcela · Paulo Henrique

---

<div align="center">

*Projeto real para cliente real — do campo ao deploy 🚀*

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=2&height=100&section=footer" width="100%"/>

</div>
