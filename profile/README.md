# Wiliam De Schepper

[![Linkedin Badge](https://img.shields.io/badge/-willdeschepper-2986cc?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/willdeschepper/)](https://www.linkedin.com/in/willdeschepper/)
[![npm](https://img.shields.io/badge/-npm-CB3837?style=flat-square&logo=npm&logoColor=white&link=https://www.npmjs.com/~4rweb)](https://www.npmjs.com/~4rweb)
[![Medium](https://img.shields.io/badge/-Medium-000000?style=flat-square&logo=medium&logoColor=white&link=https://medium.com/@willdeschepper)](https://medium.com/@willdeschepper)

**Tech Lead Full Stack** com mais de 20 anos em tecnologia, sendo **mais de 14 anos** construindo produtos digitais para healthcare e pharma.

Hoje atuo como Tech Lead hands-on na Float Health, liderando arquitetura e desenvolvimento enquanto continuo escrevendo código todos os dias.

Stack principal: **TypeScript, React, Next.js, Node.js e NestJS**, com arquitetura full-stack, APIs, PostgreSQL, Redis/BullMQ, WebSockets e integrações enterprise.

Nos últimos anos venho construindo sistemas de **AI com guardrails**: agentes, orquestração multi-agente e MCP. Minha tese é simples: a IA propõe, o código determinístico decide, o humano aprova.

---

## Projetos em destaque

### [MuAiFlow](https://github.com/4rweb/MuAiFlow)
Framework open source de orquestração multi-agente, publicado no npm.

Um agente planeja, um **segundo agente** revisa o plano, o humano aprova, e só então a execução acontece. A aprovação humana é garantida pela arquitetura, não por convenção: nenhum agente consegue marcar um plano como aprovado.

CLI própria, extensão para VS Code, sistema de skills instaláveis e roteamento por tier de modelo. Agnóstico de fornecedor, funciona com Claude Code, Codex CLI e outros agentes.

`TypeScript` `Node.js` `CLI` `VS Code Extension` `MIT`

### [AI Medical Review](https://github.com/4rweb/ai-medical-review)
Agente de pré-triagem clínica pelo Protocolo de Manchester. Construído para o Global AI Hackathon (Qwen Cloud, Track 4).

O foco não foi "integrar um LLM". Foi construir um sistema de AI em que dá para confiar num contexto clínico. Arquitetura anti-alucinação em cinco camadas, incluindo um **validador determinístico que sobrepõe a decisão da AI** em casos críticos, com trilha de auditoria em banco.

Servidor MCP como host canônico das ferramentas clínicas. Decisão registrada em ADR: sem RAG vetorial, conhecimento crítico vira código auditável em vez de memória de modelo.

`TypeScript` `NestJS` `React` `MCP` `Function Calling` `Drizzle` `PostgreSQL` `MIT`

### TeamSync
Plataforma de gestão de squads, construída do zero e em produção.

Monorepo com três aplicações consumindo uma única API em arquitetura de camadas: web em React 19, API em Express 5 e cliente desktop em Tauri com Rust. RBAC sempre revalidado no backend, autenticação corporativa via Microsoft Entra ID, webhooks do GitHub com validação de assinatura sobre o corpo cru, jobs agendados e graceful shutdown.

Testes em três níveis, com validação automatizada no build.

`React 19` `Express 5` `PostgreSQL` `Drizzle` `Tauri` `Rust` `Playwright`

---

## Stack

**Linguagens**

![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

**Frontend**

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Next.js](https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white)
![TanStack](https://img.shields.io/badge/tanstack-%23FF4154.svg?style=for-the-badge&logo=reactquery&logoColor=white)
![Vue.js](https://img.shields.io/badge/vuejs-%2335495e.svg?style=for-the-badge&logo=vuedotjs&logoColor=%234FC08D)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-%23000000.svg?style=for-the-badge&logo=shadcnui&logoColor=white)
![Radix UI](https://img.shields.io/badge/radix%20ui-161618.svg?style=for-the-badge&logo=radixui&logoColor=white)
![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)

**Backend**

![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![NestJS](https://img.shields.io/badge/nestjs-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![Express](https://img.shields.io/badge/express-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![Fastify](https://img.shields.io/badge/fastify-%23000000.svg?style=for-the-badge&logo=fastify&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io-black?style=for-the-badge&logo=socket.io&badgeColor=010101)
![GraphQL](https://img.shields.io/badge/-GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white)

**Dados**

![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![Drizzle](https://img.shields.io/badge/Drizzle-3982CE?style=for-the-badge&logo=Drizzle&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)

**AI**

![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-74aa9c?style=for-the-badge&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=for-the-badge&logo=modelcontextprotocol&logoColor=white)

**Testes e Qualidade**

![Vitest](https://img.shields.io/badge/vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white)
![Jest](https://img.shields.io/badge/-jest-%23C21325?style=for-the-badge&logo=jest&logoColor=white)
![Playwright](https://img.shields.io/badge/playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![Testing Library](https://img.shields.io/badge/-TestingLibrary-%23E33332?style=for-the-badge&logo=testing-library&logoColor=white)

**Cloud e DevOps**

![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=Cloudflare&logoColor=white)
![Railway](https://img.shields.io/badge/railway-%230B0D0E.svg?style=for-the-badge&logo=railway&logoColor=white)

---

## Portfólio

**React / Next.js**
- [Three4 Academy](https://three4-front.vercel.app/)
- [Masterclass Digital Design](https://masterclassdigitaldesign.vercel.app/)
- [Blathy](https://blathy.vercel.app/)
- [Luz](https://luz-nextjs.vercel.app/)
- [Mumu Generator](https://mumu-generator.vercel.app/)

**Vue**
- [4RWeb](https://www.4rweb.net)

<details>
<summary><b>Arquivo histórico</b> (Flash, jQuery e projetos antigos)</summary>

<br>

Projetos de fases anteriores da carreira, mantidos como registro. Alguns rodam hoje via Ruffle.

- [Ability](https://ability-game-flash.vercel.app/) — jogo de plataforma que criei em ActionScript
- [Cinamaker](https://cinamaker.vercel.app/)
- [Flash Sites](https://flashsites-eight.vercel.app/)
- [Programa Viva](https://www.programaviva.com.br/)
- [Receita de Vida](https://receitadevida.com.br/)
- [Grupo Almah](https://www.grupoalmah.com.br)
- [Fibromialgia Diagnóstico](https://fibromialgiadiagnostico.com.br/) — Angular

</details>

---

## Estatísticas

<img src="https://github-readme-stats.vercel.app/api?username=4rweb&show_icons=true&theme=tokyonight&hide_border=false&include_all_commits=true&count_private=true" alt="Estatísticas do GitHub de Wiliam" width="450" />

<img src="https://github-readme-stats.vercel.app/api/top-langs?username=4rweb&layout=compact&theme=tokyonight&include_all_commits=true&count_private=true&langs_count=8" alt="Linguagens mais usadas" width="350" />

<img src="https://streak-stats.demolab.com?user=4rweb&theme=tokyonight&date_format=j%20M%5B%20Y%5D" alt="Sequência de contribuições" width="450" />
