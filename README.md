# 🛡️ Cybersecurity & SOC Engineering Portfolio

[![Next.js 15](https://img.shields.io/badge/Next.js_15-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com/)
[![Security Focus](https://img.shields.io/badge/Focus-Blue_Team_%7C_SOC-blue?style=for-the-badge&logo=shield)](https://github.com/Leanszz)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

> Repositório oficial do meu Portfólio Profissional voltado para **Operações de Segurança (SOC)**, **Análise de Incidentes**, **Análise Forense de Redes** e **Automação de Segurança**. Desenvolvido com **Next.js 15 (App Router)**, **TypeScript** e **Tailwind CSS**.

---

## 🔍 Visão Geral (Overview)

Este repositório contém o código-fonte do portfólio interativo de **Leandro Andrade**, estudante de Segurança Cibernética na FIAP e profissional de TI com sólida experiência em suporte técnico, infraestrutura corporativa e resposta a incidentes.

O objetivo principal desta aplicação web é consolidar e expor de forma transparente:
* **Laboratórios Práticos de Cibersegurança:** Projetos hands-on de análise de pacotes PCAP, automação com Python e Scapy, hardening de Active Directory e auditoria de sistemas via PowerShell.
* **Métricas de Infraestrutura & SOC:** Casos de estudo focados na redução do tempo de resposta (MTTR), mapeamento de superfície de ataque e prevenção de falhas de causa raiz.
* **Trajetória e Certificações:** Evolução técnica contínua alinhada ao roadmap para atuar como Analista de SOC / Blue Team Specialist.

---

## ⚡ Tech Stack & Ferramentas

Uma visão categorizada das tecnologias utilizadas tanto para a **construção da aplicação web** quanto para a **execução dos laboratórios de segurança**.

### 💻 Desenvolvimento & Web Engineering
| Categoria | Tecnologias Utilizadas |
| :--- | :--- |
| **Framework Web** | Next.js 15 (App Router, Server Components) |
| **Linguagem** | TypeScript |
| **Estilização** | Tailwind CSS, PostCSS, Autoprefixer |
| **Animações & Ícones** | Framer Motion, Lucide React |
| **Deployment** | Vercel Edge Network |

### 🚨 Segurança, Infraestrutura & Automação (Blue Team / SOC)
| Domínio | Ferramentas & Tecnologias |
| :--- | :--- |
| **Análise de Tráfego & Forense** | Wireshark, TShark, Network Forensics, Análise de Arquivos PCAP |
| **Mapeamento & Reconhecimento** | Nmap, Scapy, OWASP Top 10 |
| **Infraestrutura Corporativa** | Active Directory (FSMO, GPO Hardening, Event Log Auditing), VMware, Linux (Debian/Ubuntu/CentOS), Windows Server |
| **Scripting & Automação** | Python (`socket`, `requests`, `scapy`), PowerShell (`Get-*`, `Import-*`, auditoria de módulos), Bash |
| **Gestão & Processos** | ITIL v4, SLA, Análise de Causa Raiz, Documentação Técnica (SOPs) |

---

## 📁 Estrutura do Repositório

A arquitetura do projeto segue o padrão do **Next.js 15 App Router**, estruturada de forma modular e altamente escalável:

```text
cybersecurity-portfolio/
├── public/
│   ├── favicon.ico
│   └── resume.pdf                 # Currículo oficial em PDF para download
├── src/
│   ├── app/
│   │   ├── globals.css            # Configurações globais do Tailwind CSS
│   │   ├── layout.tsx             # Root Layout, font loaders e SEO Metadata
│   │   ├── page.tsx               # Página principal (Single Page Application)
│   │   └── sitemap.ts             # Gerador de sitemap para SEO
│   ├── components/
│   │   ├── layout/
│   │   │   ├── Footer.tsx         # Rodapé com redes e links de contato
│   │   │   └── Navbar.tsx         # Barra de navegação responsiva com smooth scroll
│   │   ├── sections/
│   │   │   ├── AboutSection.tsx            # Resumo profissional e trajetória
│   │   │   ├── CertificationsSection.tsx   # Certificações obtidas e em andamento
│   │   │   ├── ContactSection.tsx          # Formulário/Links diretos de contato
│   │   │   ├── ExperienceSection.tsx       # Histórico de atuação em TI/Suporte
│   │   │   ├── HeroSection.tsx             # Apresentação inicial e call-to-action
│   │   │   ├── ProjectsSection.tsx         # Vitrine dos laboratórios de segurança
│   │   │   ├── RoadmapSection.tsx          # Certificações e metas até 2028
│   │   │   └── SkillsSection.tsx           # Hard/Soft skills divididas por categoria
│   │   └── SeoSchema.tsx          # Injeção de dados estruturados JSON-LD (Schema.org)
│   └── lib/
│       └── resumeData.ts          # Arquivo centralizador de dados e projetos (Single Source of Truth)
├── tailwind.config.ts             # Customização de temas e fontes
├── tsconfig.json                  # Configuração estrita do TypeScript
└── package.json                   # Dependências e scripts do projeto
