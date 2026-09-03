# Wiliam De Schepper

<a href="https://www.linkedin.com/in/willdeschepper/" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/-willdeschepper-2986cc?style=flat-square&amp;logo=linkedin&amp;logoColor=white" alt="LinkedIn Badge" /></a>
<a href="https://www.npmjs.com/~4rweb" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/-npm-CB3837?style=flat-square&amp;logo=npm&amp;logoColor=white" alt="npm" /></a>
<a href="https://medium.com/@willdeschepper" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/-Medium-000000?style=flat-square&amp;logo=medium&amp;logoColor=white" alt="Medium" /></a>

**Tech Lead Full Stack** com mais de 20 anos em tecnologia, sendo **mais de 14 anos** construindo produtos digitais para healthcare e pharma.

Hoje atuo como Tech Lead hands-on na Float Health, liderando arquitetura e desenvolvimento enquanto continuo escrevendo código todos os dias.

Minha stack atual é **TypeScript, React, Next.js, Node.js e NestJS**, com arquitetura full stack, APIs, PostgreSQL, Redis/BullMQ, WebSockets e integrações enterprise.

Minha experiência também inclui **desenvolvimento mobile com React Native para iOS e Android**, da arquitetura à publicação nas lojas. No **MemoriaViva**, trabalhei com operação offline-first, persistência local e sincronização com o backend, conectando o aplicativo de cuidadores a um portal utilizado por profissionais de saúde.

Parte dos produtos que desenvolvi em healthcare e pharma tem acesso restrito por contratos e compliance. O portfólio reúne projetos e demonstrações que posso compartilhar publicamente.

Nos últimos anos venho construindo sistemas de **AI com guardrails**: agentes, orquestração multi-agente e MCP. Minha tese é simples: a IA propõe, o código determinístico decide, o humano aprova.

---

## Projetos em destaque

### MemoriaViva — Programa Alzheimer LIBBS

Aplicativo **React Native para iOS e Android** desenvolvido para apoiar cuidadores de pacientes com Alzheimer, integrado a um backend Node.js e a um portal utilizado por profissionais de saúde.

Atuei de ponta a ponta, da arquitetura ao desenvolvimento e à publicação nas duas lojas. O aplicativo permite registrar medicamentos, sinais vitais, quedas e outros eventos mesmo sem conexão: os dados são persistidos localmente e sincronizados em lote com o backend quando a rede retorna.

O produto começou com um MVP controlado de 10 pacientes e 10 enfermeiros e evoluiu por meio de rollout progressivo. O principal desafio de engenharia foi manter a continuidade dos registros no dia a dia do cuidado, inclusive em cenários de conectividade instável.

**Stack original:** `React Native` `React Navigation` `Redux/Redux-Saga` `AsyncStorage` `Node.js` `REST APIs` `Jest`

O aplicativo original não está mais disponível nas lojas. Para apresentar suas telas e fluxos, disponibilizo uma demonstração interativa por meio de um protótipo navegável.

<a href="https://native-apps-three.vercel.app/memoria-viva/" target="_blank" rel="noopener noreferrer"><strong>Ver demonstração interativa →</strong></a>

### Protocolo da Dor — apoio à avaliação de fibromialgia

Aplicativo de apoio a profissionais de saúde na avaliação e abordagem da fibromialgia. A interface reúne um mapa corporal interativo para seleção das áreas dolorosas e apresenta o Índice de Dor Generalizada (IDG), a Escala de Gravidade dos Sintomas (EGS) e a distribuição da dor por regiões.

O fluxo organiza os parâmetros informados e apresenta uma classificação como apoio complementar ao raciocínio clínico. Também reúne seções de abordagem sistêmica, encaminhamento à psiquiatria, terapêutica e referências bibliográficas.

**Stack original:** `React Native` `React Navigation` `Node.js` `REST APIs` `Jest`

<a href="https://native-apps-three.vercel.app/protocolo-da-dor/" target="_blank" rel="noopener noreferrer"><strong>Ver demonstração interativa →</strong></a>

### Tarja Rosa — saúde feminina, autocuidado e lembretes via WhatsApp

Aplicativo de saúde e bem-estar feminino para a Libbs, reunindo conteúdo educativo, autocuidado e apoio à rotina de medicamentos em uma experiência mobile com temas claro e escuro.

O **TarjaBot** permite configurar lembretes de tomada de medicamentos pelo WhatsApp e registrar as confirmações da usuária. Um painel apresenta os indicadores de mensagens enviadas, recebidas e confirmadas, com consulta por período.

A experiência inclui **podcasts**, dicas e notícias sobre sexualidade, contracepção e atualidades, além de conteúdos de alimentação, exercícios, alongamento, meditação e yoga. Os conteúdos são organizados por categorias, com recursos de busca, curtidas e favoritos.

O **TarjaMoji** acrescenta uma camada de personalização: a usuária monta seu avatar escolhendo cabelo, cor, tom de pele e outros traços, com figurinhas que também aparecem nas conversas do TarjaBot.

**Stack original:** `React Native` `React Navigation` `Node.js` `REST APIs` `Jest`

**Recursos e integrações:** `WhatsApp` `Lembretes agendados` `Podcasts` `Visualização de dados` `Temas claro/escuro` `Avatares personalizáveis`

O aplicativo original não está mais disponível nas lojas. A demonstração interativa preserva suas interfaces e fluxos para apresentação do projeto.

<a href="https://native-apps-three.vercel.app/tarja-rosa/" target="_blank" rel="noopener noreferrer"><strong>Ver demonstração interativa →</strong></a>

### <a href="https://github.com/willdeschepper/MuAiFlow" target="_blank" rel="noopener noreferrer">MuAiFlow</a>

Framework open source de orquestração multi-agente, publicado no npm.

Um agente planeja, um **segundo agente** revisa o plano, o humano aprova, e só então a execução acontece. A aprovação humana é garantida pela arquitetura, não por convenção: nenhum agente consegue marcar um plano como aprovado.

CLI própria, extensão para VS Code, sistema de skills instaláveis e roteamento por tier de modelo. Agnóstico de fornecedor, funciona com Claude Code, Codex CLI e outros agentes.

`TypeScript` `Node.js` `CLI` `VS Code Extension` `MIT`

### <a href="https://github.com/willdeschepper/ai-medical-review" target="_blank" rel="noopener noreferrer">AI Medical Review</a>

Agente de pré-triagem clínica pelo Protocolo de Manchester. Construído para o Global AI Hackathon (Qwen Cloud, Track 4).

O foco não foi "integrar um LLM". Foi construir mecanismos de controle para AI em um contexto clínico. Arquitetura anti-alucinação em cinco camadas, incluindo um **validador determinístico que sobrepõe a decisão da AI** em casos críticos, com trilha de auditoria em banco.

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
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

**Frontend**

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Next.js](https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white)
![TanStack](https://img.shields.io/badge/tanstack-%23FF4154.svg?style=for-the-badge&logo=reactquery&logoColor=white)
![Vue.js](https://img.shields.io/badge/vuejs-%2335495e.svg?style=for-the-badge&logo=vuedotjs&logoColor=%234FC08D)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwindcss&logoColor=white)
![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-%23000000.svg?style=for-the-badge&logo=shadcnui&logoColor=white)
![Radix UI](https://img.shields.io/badge/radix%20ui-161618.svg?style=for-the-badge&logo=radixui&logoColor=white)
![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)

**Mobile**

![React Native](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![React Navigation](https://img.shields.io/badge/React_Navigation-6B52AE?style=for-the-badge&logo=reactnavigation&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=for-the-badge&logo=redux&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=black)
![iOS](https://img.shields.io/badge/iOS-000000?style=for-the-badge&logo=apple&logoColor=white)

Arquitetura offline-first, persistência local, sincronização com APIs e publicação para iOS e Android. Experiência com React Navigation, Redux/Redux-Saga e AsyncStorage, além de projetos híbridos com PhoneGap.

**Backend**

![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![NestJS](https://img.shields.io/badge/nestjs-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![Express](https://img.shields.io/badge/express-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![Fastify](https://img.shields.io/badge/fastify-%23000000.svg?style=for-the-badge&logo=fastify&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io-black?style=for-the-badge&logo=socket.io&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white)

**Dados**

![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![Drizzle](https://img.shields.io/badge/Drizzle-3982CE?style=for-the-badge&logo=drizzle&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-%23000f.svg?style=for-the-badge&logo=mysql&logoColor=white)

**AI**

![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-74aa9c?style=for-the-badge&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=for-the-badge&logo=modelcontextprotocol&logoColor=white)

**Testes e Qualidade**

![Vitest](https://img.shields.io/badge/vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white)
![Jest](https://img.shields.io/badge/jest-%23C21325?style=for-the-badge&logo=jest&logoColor=white)
![Playwright](https://img.shields.io/badge/playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![Testing Library](https://img.shields.io/badge/Testing_Library-%23E33332?style=for-the-badge&logo=testinglibrary&logoColor=white)

**Cloud e DevOps**

![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)
![Railway](https://img.shields.io/badge/railway-%230B0D0E.svg?style=for-the-badge&logo=railway&logoColor=white)

---

## Portfólio

### Aplicativos mobile

Aplicativos que desenvolvi e que foram publicados nas lojas. Como hoje não estão mais disponíveis para download, disponibilizo demonstrações web e protótipos navegáveis para apresentar suas interfaces e fluxos.

| Projeto | Demonstração |
| --- | --- |
| **HER2** | <a href="https://native-apps-three.vercel.app/her2/" target="_blank" rel="noopener noreferrer">Abrir demonstração web</a> — interface interativa com seleção de características de perfis clínicos. |
| **Lanxess** | <a href="https://native-apps-three.vercel.app/lanxess/" target="_blank" rel="noopener noreferrer">Ver demonstração interativa</a> |

Explore também os projetos em **React Native** — MemoriaViva, Protocolo da Dor e Tarja Rosa — na seção <a href="#projetos-em-destaque">Projetos em destaque ↑</a>.

### React / Next.js

- <a href="https://three4-front.vercel.app/" target="_blank" rel="noopener noreferrer">Three4 Academy</a>
- <a href="https://masterclassdigitaldesign.vercel.app/" target="_blank" rel="noopener noreferrer">Masterclass Digital Design</a>
- <a href="https://blathy.vercel.app/" target="_blank" rel="noopener noreferrer">Blathy</a>
- <a href="https://luz-nextjs.vercel.app/" target="_blank" rel="noopener noreferrer">Luz</a>
- <a href="https://mumu-generator.vercel.app/" target="_blank" rel="noopener noreferrer">Mumu Generator</a>

### Vue

- <a href="https://www.4rweb.net" target="_blank" rel="noopener noreferrer">4RWeb</a>

<details>
<summary><b>Arquivo histórico</b> (Flash, jQuery e projetos antigos)</summary>

<br>

Projetos de fases anteriores da carreira, mantidos como registro. Alguns rodam hoje via Ruffle.

- <a href="https://ability-game-flash.vercel.app/" target="_blank" rel="noopener noreferrer">Ability</a> — jogo de plataforma que criei em ActionScript
- <a href="https://cinamaker.vercel.app/" target="_blank" rel="noopener noreferrer">Cinamaker</a>
- <a href="https://flashsites-eight.vercel.app/" target="_blank" rel="noopener noreferrer">Flash Sites</a>
- <a href="https://www.programaviva.com.br/" target="_blank" rel="noopener noreferrer">Programa Viva</a>
- <a href="https://receitadevida.com.br/" target="_blank" rel="noopener noreferrer">Receita de Vida</a>
- <a href="https://www.grupoalmah.com.br" target="_blank" rel="noopener noreferrer">Grupo Almah</a>
- <a href="https://fibromialgiadiagnostico.com.br/" target="_blank" rel="noopener noreferrer">Fibromialgia Diagnóstico</a> — Angular

</details>

---

## Estatísticas

![Linguagens de Wiliam De Schepper](https://github-readme-stats.vercel.app/api/top-langs?username=willdeschepper&show_icons=true&locale=pt-br&layout=compact&theme=tokyonight&include_all_commits=true&count_private=true)

<img width="500" src="https://github-readme-stats-4rweb.vercel.app/api?username=willdeschepper&theme=tokyonight&hide_border=false&include_all_commits=true&count_private=true" alt="Estatísticas de Wiliam De Schepper" />

<a href="https://github.com/willdeschepper" target="_blank" rel="noopener noreferrer"><img src="https://github-readme-streak-stats-4rweb.vercel.app?user=willdeschepper&amp;theme=tokyonight&amp;date_format=j%20M%5B%20Y%5D" alt="GitHub Streak" /></a>

![Atividade de Wiliam De Schepper](https://github-readme-activity-graph.vercel.app/graph?username=willdeschepper&theme=github-compact)
