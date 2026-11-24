<div align="center">

<img width="100%" alt="Rafael Maia" src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,45:5B21B6,100:06B6D4&height=230&section=header&text=Rafael%20Maia&fontSize=78&fontColor=F8FAFC&animation=twinkling&fontAlignY=35&desc=Back-end%20que%20sabe%20onde%20o%20c%C3%B3digo%20roda&descAlignY=60&descSize=22&descColor=BAE6FD" />

<a href="https://github.com/rafaelmaia-dev">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3200&pause=1100&color=38BDF8&center=true&vCenter=true&width=680&lines=Do+cabo+de+rede+ao+c%C3%B3digo+back-end;Python+%C2%B7+FastAPI+%C2%B7+PostgreSQL+%C2%B7+Docker;Construindo+o+AgentWire+(pipeline+determin%C3%ADstico+de+IA);Aberto+a+est%C3%A1gio+ou+vaga+j%C3%BAnior+em+back-end" alt="Typing SVG" />
</a>

<br/>

[https://img.shields.io/badge/status-aberto%20a%20est%C3%A1gio%20ou%20j%C3%BAnior-22C55E?style=for-the-badge&labelColor=0F172A]
[https://img.shields.io/badge/foco-Back--end%20%7C%20APIs%20%7C%20Seguran%C3%A7a-7C3AED?style=for-the-badge&labelColor=0F172A]
[https://img.shields.io/badge/Brasil-06B6D4?style=for-the-badge&logo=googlemaps&logoColor=white&labelColor=0F172A]

<br/>

[[https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white]](https://www.linkedin.com/in/rafael-maia-508554232)
[[https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white]](https://github.com/rafaelmaia-dev)
[[https://img.shields.io/badge/Projeto%20Destaque-AgentWire-8B5CF6?style=for-the-badge&logo=telegram&logoColor=white]](https://github.com/rafaelmaia-dev/bot_noticias_ia)

</div>

<br/>

## ⚡ Sobre mim

<table>
<tr>
<td width="54%" valign="top">

### Do cabo ao código

Antes de subir meu primeiro endpoint, eu já estava na linha de frente vendo **onde o software é instalado, em que rede ele roda e o que acontece quando algo cai**.

- **Hoje:** Auxiliar de Instalação na **Procfit**, no time de instalações de PDV, pré-venda e VPNs.
- **Antes:** Estagiário de Infraestrutura no **Instituto Almai** (redes, suporte, VoIP e sistemas).
- **Formação:** Sistemas de Informação na **FALS** (6º semestre · previsão dez/2027).
- **Direção:** Desenvolvimento **Back-end** com foco em APIs, bancos relacionais, containers e segurança.

> [!IMPORTANT]
> **Buscando oportunidade:** estágio ou vaga júnior em desenvolvimento back-end.

</td>
<td width="46%" valign="top">

```bash
$ systemctl status rafael.service

● rafael.service - Back-end Dev
   Loaded: FALS · SI (6º sem.)
   Active: active (running)
     Role: Procfit · PDV & VPNs
    Focus: APIs · Dados · Segurança
    Build: AgentWire (Telegram Bot)
       OS: Zorin OS · JetBrains Mono
    Games: Resident Evil 4 Remake
```

</td>
</tr>
</table>

<br/>

## 🚀 Projeto em Destaque — AgentWire

> **Bot no Telegram que mantém devs e vibe coders por dentro das novidades dos agentes de código** (Claude Code, Codex, DeepSeek, Anthropic, OpenAI e afins), cobrindo mudanças técnicas, financeiras e sociais.

[https://img.shields.io/badge/status-em%20desenvolvimento-F59E0B?style=flat-square&labelColor=0F172A]
[https://img.shields.io/github/last-commit/rafaelmaia-dev/bot_noticias_ia?style=flat-square&label=%C3%BAltimo%20commit&labelColor=0F172A&color=06B6D4]
[https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white]
[https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white]
[https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white]
[[https://img.shields.io/badge/Ver%20Reposit%C3%B3rio-181717?style=flat-square&logo=github&logoColor=white]](https://github.com/rafaelmaia-dev/bot_noticias_ia)

**O problema:** acompanhar lançamentos e mudanças de agentes de IA espalhados em blogs, repositórios e redes sociais consome tempo demais. O **AgentWire** coleta, deduplica, resume e entrega direto no Telegram com link da fonte original — pronto para rodar **local/self-hosted**.

```mermaid
flowchart LR
    subgraph IN["🌐 Fontes"]
        A["RSS · GitHub<br/>HN · Hugging Face"]
    end
    subgraph PIPE["⚙️ Pipeline Determinístico"]
        B["Parser +<br/>Deduplicação"]
        C[("PostgreSQL<br/>SQLAlchemy Async")]
        D["Resumo<br/>Groq API"]
    end
    subgraph OUT["📡 Entrega & API"]
        E["Telegram Bot"]
        F["API REST<br/>FastAPI"]
    end

    A --> B --> C
    C --> D --> E
    C <--> F

    classDef neon fill:#4C1D95,stroke:#A78BFA,color:#F8FAFC,stroke-width:1.5px
    classDef cyan fill:#0E7490,stroke:#38BDF8,color:#F8FAFC,stroke-width:1.5px
    class A,B,D,E,F neon
    class C cyan
    style IN fill:#0F172A,stroke:#38BDF8,color:#BAE6FD
    style PIPE fill:#0F172A,stroke:#8B5CF6,color:#DDD6FE
    style OUT fill:#0F172A,stroke:#22C55E,color:#BBF7D0
```

<sub>As fontes além de RSS fazem parte do roadmap · desenvolvido com apoio do Antigravity.</sub>

| Pilar de Engenharia | Decisão Aplicada |
|:---|:---|
| 🧠 **Determinismo acima de hype** | Não é um agente autônomo: é um pipeline determinístico e auditável *sobre* agentes, usando LLM (`Groq API`) só para resumir. |
| 🧩 **Desacoplamento real** | **API REST (`FastAPI`)** e **worker (`APScheduler`)** separados, compartilhando o mesmo **PostgreSQL**. |
| 🔒 **Self-hosted sem dor de cabeça** | Integração planejada com Hugging Face via polling (Hub API + RSS), descartando webhooks públicos. |
| 🐳 **Qualidade e portabilidade** | Empacotado em **Docker** com testes automatizados e de regressão em evolução. |

<br/>

## 🛠️ Outros Projetos & Experiências Práticas

<table>
<tr>
<td width="50%" valign="top">

### 🔌 [API Google](https://github.com/rafaelmaia-dev/api-google)
Script em Python que realiza requisições HTTP (`GET`) para exercitar consumo, parsing e tratamento de respostas de APIs externas.

[https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white]
[https://img.shields.io/badge/HTTP%20%26%20REST-7C3AED?style=flat-square]

👉 [**Explorar repositório**](https://github.com/rafaelmaia-dev/api-google)

</td>
<td width="50%" valign="top">

### 🧮 [Calculadora CLI + CI/CD](https://github.com/rafaelmaia-dev/calculadora-while)
Aplicação interativa de terminal em Python com laços `while` para validação de entrada, controle de fluxo e automação de CI/CD.

[https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white]
[https://img.shields.io/badge/CI%2FCD-06B6D4?style=flat-square&logo=githubactions&logoColor=white]

👉 [**Explorar repositório**](https://github.com/rafaelmaia-dev/calculadora-while)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🤖 Chatbot de Telegram (Caso Técnico Nola)
Fluxo automatizado integrando **N8N**, **Groq** e **Google Sheets** para atendimento e processamento de mensagens via Telegram.

[https://img.shields.io/badge/N8N-EA4B71?style=flat-square&logo=n8n&logoColor=white]
[https://img.shields.io/badge/Groq%20API-F59E0B?style=flat-square]
[https://img.shields.io/badge/Telegram-26A5E4?style=flat-square&logo=telegram&logoColor=white]

</td>
<td width="50%" valign="top">

### 🌐 Infra, Redes & Automações
Experiência prática com **VPNs**, **Wireshark**, **VoIP (Yeastar/Linkus)**, **SharePoint**, **TOTVS RH**, além de estudos com integração **ClickUp–Obsidian** e projeto acadêmico em **Java**.

[https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black]
[https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white]
[https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white]

</td>
</tr>
</table>

<br/>

## 🧰 Arsenal Tecnológico

<div align="center">

<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=py,fastapi,django,c,postgres,mysql,docker,linux,git,github,githubactions,vscode,obsidian&theme=dark&perline=7" alt="Tech Stack" />
</a>

</div>

<br/>

```mermaid
flowchart TB
    subgraph L1["🟣 APLICAÇÃO & APIs"]
        direction LR
        A1["Python"]
        A2["FastAPI"]
        A3["Django"]
        A4["C"]
    end
    subgraph L2["🔵 DADOS & PERSISTÊNCIA"]
        direction LR
        B1["PostgreSQL"]
        B2["MySQL"]
        B3["SQLAlchemy Async"]
    end
    subgraph L3["🩵 QUALIDADE, CI/CD & SEGURANÇA"]
        direction LR
        C1["Pytest"]
        C2["Docker"]
        C3["GitHub Actions"]
        C4["JWT · OAuth2 · Trivy"]
    end
    subgraph L4["🟢 SISTEMAS & REDES"]
        direction LR
        D1["Linux (Zorin/Ubuntu)"]
        D2["VPN"]
        D3["Wireshark"]
        D4["TCP/IP · DNS · DHCP"]
    end

    A1 ~~~ A2 ~~~ A3 ~~~ A4
    B1 ~~~ B2 ~~~ B3
    C1 ~~~ C2 ~~~ C3 ~~~ C4
    D1 ~~~ D2 ~~~ D3 ~~~ D4
    L1 ~~~ L2 ~~~ L3 ~~~ L4

    classDef l1 fill:#6D28D9,stroke:#A78BFA,color:#fff
    classDef l2 fill:#4338CA,stroke:#818CF8,color:#fff
    classDef l3 fill:#0E7490,stroke:#38BDF8,color:#fff
    classDef l4 fill:#15803D,stroke:#4ADE80,color:#fff
    class A1,A2,A3,A4 l1
    class B1,B2,B3 l2
    class C1,C2,C3,C4 l3
    class D1,D2,D3,D4 l4
    style L1 fill:#0F172A,stroke:#8B5CF6,stroke-width:2px,color:#DDD6FE
    style L2 fill:#0F172A,stroke:#6366F1,stroke-width:2px,color:#C7D2FE
    style L3 fill:#0F172A,stroke:#06B6D4,stroke-width:2px,color:#BAE6FD
    style L4 fill:#0F172A,stroke:#22C55E,stroke-width:2px,color:#BBF7D0
```

<div align="center">
  <sub><strong>Ambiente diário:</strong> Zorin OS · VSCode · Antigravity · GitHub Copilot · DBeaver · Obsidian · JetBrains Mono</sub>
</div>

<br/>

## 🗺️ Trajetória & Foco Atual

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'git0': '#06B6D4', 'git1': '#8B5CF6', 'commitLabelColor': '#F8FAFC', 'commitLabelBackground': '#0F172A'}, 'gitGraph': {'showBranches': false, 'rotateCommitLabel': true}}}%%
gitGraph
    commit id: "FALS · Sistemas de Informação"
    commit id: "Instituto Almai · Infra e Redes"
    branch back-end
    checkout back-end
    commit id: "Python e FastAPI"
    commit id: "AgentWire"
    checkout main
    commit id: "Procfit · PDV e VPNs"
    checkout back-end
    commit id: "FastAPI Assíncrono (nov/2026)"
    commit id: "Próximo: vaga júnior" type: HIGHLIGHT
```

- [x] **FastAPI: APIs Modernas e Assíncronas com Python** — concluído em nov/2026
- [ ] **SQLAlchemy 2.0 assíncrono + `asyncpg` + Alembic**
- [ ] **Testes automatizados e de regressão com Pytest**
- [ ] **CI/CD e segurança com GitHub Actions, SonarCloud e Trivy**
- [ ] **Concluir o pipeline principal do AgentWire**

<br/>

## 📊 Atividade no GitHub

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=rafaelmaia-dev&show_icons=true&bg_color=0F172A&title_color=A78BFA&icon_color=38BDF8&text_color=E2E8F0&border_color=312E81&border_radius=10&hide_border=false" alt="GitHub Stats de Rafael Maia" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=rafaelmaia-dev&layout=compact&bg_color=0F172A&title_color=A78BFA&text_color=E2E8F0&border_color=312E81&border_radius=10&hide_border=false" alt="Linguagens mais usadas" />

</div>

<br/>

## 🎓 Formação & Certificações

| Formação | Instituição | Status |
|:---|:---|:---|
| **Sistemas de Informação** | FALS · Faculdade do Litoral Sul Paulista | [https://img.shields.io/badge/em%20andamento-F59E0B?style=flat-square&labelColor=0F172A] 6º sem. · dez/2027 |
| **FastAPI: APIs Modernas e Assíncronas com Python** | Udemy · Geek University · 12,5 h | [https://img.shields.io/badge/conclu%C3%ADdo-22C55E?style=flat-square&labelColor=0F172A] nov/2026 |
| **Redes de Computadores com Wireshark** | Udemy | [https://img.shields.io/badge/curso%20extra-06B6D4?style=flat-square&labelColor=0F172A] |
| **Git e GitHub** | Udemy | [https://img.shields.io/badge/curso%20extra-7C3AED?style=flat-square&labelColor=0F172A] |
| **Inglês** | CNA Master in English | [https://img.shields.io/badge/idioma-4F46E5?style=flat-square&labelColor=0F172A] |

<br/>

## 🤝 Vamos conversar!

> [!TIP]
> O jeito mais rápido de falar comigo é pelo **LinkedIn**. Se você é recrutador, tech lead ou dev querendo trocar ideia sobre **vagas de back-end, infraestrutura ou o AgentWire**, chama lá!

<div align="center">

[[https://img.shields.io/badge/Chamar%20no%20LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white]](https://www.linkedin.com/in/rafael-maia-508554232)
[[https://img.shields.io/badge/Seguir%20no%20GitHub-181717?style=for-the-badge&logo=github&logoColor=white]](https://github.com/rafaelmaia-dev)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:06B6D4,55:5B21B6,100:0F172A&height=120&section=footer" width="100%" />

</div>
