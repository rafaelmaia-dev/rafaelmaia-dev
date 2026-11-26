<div align="center">

<img width="100%" alt="Rafael Maia — Back-end que sabe onde o código roda" src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,45:5B21B6,100:06B6D4&height=225&section=header&text=Rafael%20Maia&fontSize=76&fontColor=F8FAFC&animation=twinkling&fontAlignY=35&desc=Back-end%20que%20sabe%20onde%20o%20c%C3%B3digo%20roda&descAlignY=61&descSize=21&descColor=BAE6FD" />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=19&duration=3200&pause=1100&color=38BDF8&center=true&vCenter=true&width=720&lines=Do+cabo+de+rede+ao+c%C3%B3digo+back-end;Python+%C2%B7+FastAPI+%C2%B7+PostgreSQL+%C2%B7+Docker;Construindo+o+AgentWire+%E2%80%94+pipeline+de+IA+audit%C3%A1vel;Aberto+a+est%C3%A1gio+ou+vaga+j%C3%BAnior+em+back-end" alt="Resumo animado de Rafael Maia" />

<br/>

[https://img.shields.io/badge/status-aberto%20a%20est%C3%A1gio%20ou%20j%C3%BAnior-22C55E?style=flat-square&labelColor=0F172A]
[https://img.shields.io/badge/foco-Back--end%20%C2%B7%20APIs%20%C2%B7%20Seguran%C3%A7a-7C3AED?style=flat-square&labelColor=0F172A]
[https://img.shields.io/badge/base-Brasil-06B6D4?style=flat-square&labelColor=0F172A]

<br/>

[[https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white]](https://www.linkedin.com/in/rafael-maia-508554232)
[[https://img.shields.io/badge/Reposit%C3%B3rios-181717?style=for-the-badge&logo=github&logoColor=white]](https://github.com/rafaelmaia-dev?tab=repositories)
[[https://img.shields.io/badge/Projeto%20Destaque-AgentWire-8B5CF6?style=for-the-badge&logo=telegram&logoColor=white]](https://github.com/rafaelmaia-dev/bot_noticias_ia)

</div>

<br/>

## ⚡ Sobre mim

<table>
<tr>
<td width="55%" valign="top">

### Do cabo ao código

Quem já configurou VPN, analisou pacote no Wireshark e diagnosticou queda em produção escreve back-end pensando em **rede, falha e deploy** — não só no que funciona em `localhost`.

- **Hoje:** Auxiliar de Instalação na **Procfit**, no time de instalações de PDV, pré-venda e VPNs.
- **Antes:** Estagiário de Infraestrutura no **Instituto Almai** (redes, suporte de TI e sistemas).
- **Formação:** Sistemas de Informação na **FALS** (6º semestre · previsão dez/2027).
- **Foco:** Desenvolvimento **Back-end** com Python, APIs assíncronas, bancos relacionais, Docker e segurança.

</td>
<td width="45%" valign="top">

```bash
$ systemctl status rafael.service

● rafael.service — Back-end Dev
   Loaded:   FALS · SI (6º sem.)
   Active:   active (running)
   Role:     Procfit · PDV & VPNs
   Focus:    APIs · Dados · Segurança
   Build:    AgentWire (Telegram Bot)
   OS:       Zorin OS · JetBrains Mono
   Off-duty: Resident Evil 4 Remake
```

</td>
</tr>
</table>

> [!IMPORTANT]
> **Aberto a oportunidades:** busco estágio ou vaga júnior em desenvolvimento back-end.

<br/>

## 🚀 Projeto em Destaque — AgentWire

> **Bot no Telegram que mantém devs e vibe coders por dentro das novidades dos agentes de código** (Claude Code, Codex, DeepSeek, Anthropic, OpenAI e afins), cobrindo mudanças técnicas, financeiras e sociais.

[https://img.shields.io/badge/status-em%20desenvolvimento-F59E0B?style=flat-square&labelColor=0F172A]
[https://img.shields.io/github/last-commit/rafaelmaia-dev/bot_noticias_ia?style=flat-square&label=%C3%BAltimo%20commit&labelColor=0F172A&color=06B6D4]
[https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white&labelColor=0F172A]
[https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white&labelColor=0F172A]
[https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white&labelColor=0F172A]
[[https://img.shields.io/badge/Ver%20Reposit%C3%B3rio-181717?style=flat-square&logo=github&logoColor=white]](https://github.com/rafaelmaia-dev/bot_noticias_ia)

**O problema:** atualizações de agentes de IA saem espalhadas em blogs, repositórios e redes sociais, e acompanhar tudo consome tempo demais. O **AgentWire** coleta, deduplica, resume e entrega direto no Telegram com link da fonte original — pronto para rodar **local/self-hosted**.

```mermaid
flowchart LR
    subgraph IN["1 · FONTES"]
        A["RSS · GitHub<br/>HN · Hugging Face"]
    end
    subgraph PIPE["2 · PIPELINE DETERMINÍSTICO"]
        B["Parser +<br/>Deduplicação"]
        C[("PostgreSQL<br/>SQLAlchemy Async")]
        D["Resumo<br/>Groq API"]
    end
    subgraph OUT["3 · ENTREGA E API"]
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
| 🧠 **Determinismo acima de hype** | Escolhido de propósito no lugar de um agente autônomo: cada etapa tem entrada e saída definidas, e o LLM (`Groq API`) entra só para resumir. |
| 🧩 **Desacoplamento real** | **API REST (`FastAPI`)** e **worker (`APScheduler`)** separados sobre o mesmo **PostgreSQL** (`SQLAlchemy Async`). |
| 🔒 **Self-hosted sem expor porta** | Integração planejada com Hugging Face via polling (Hub API + RSS do blog), descartando webhooks públicos. |
| 🐳 **Qualidade e reprodutibilidade** | Empacotado em **Docker** para rodar localmente, com testes automatizados e de regressão em evolução. |

<br/>

## 🛠️ Outros Projetos & Experiências Práticas

<table>
<tr>
<td width="50%" valign="top">

### 🔌 API Google
Script em Python que executa requisições HTTP (`GET`) para exercitar consumo, parsing e tratamento de respostas de APIs externas.

[https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white]
[https://img.shields.io/badge/HTTP%20%26%20REST-7C3AED?style=flat-square]
[[https://img.shields.io/badge/Ver%20Reposit%C3%B3rio-181717?style=flat-square&logo=github&logoColor=white]](https://github.com/rafaelmaia-dev/api-google)

</td>
<td width="50%" valign="top">

### 🧮 Calculadora CLI + CI/CD
Aplicação interativa de terminal em Python com laços `while` para validação de entrada, controle de fluxo e pipeline de CI/CD.

[https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white]
[https://img.shields.io/badge/CI%2FCD-06B6D4?style=flat-square&logo=githubactions&logoColor=white]
[[https://img.shields.io/badge/Ver%20Reposit%C3%B3rio-181717?style=flat-square&logo=github&logoColor=white]](https://github.com/rafaelmaia-dev/calculadora-while)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🤖 Chatbot de Telegram · Caso Técnico Nola
Automação ponta a ponta integrando **N8N**, **Groq API** e **Google Sheets** para atendimento e processamento de mensagens no Telegram.

[https://img.shields.io/badge/tipo-caso%20t%C3%A9cnico-8B5CF6?style=flat-square&labelColor=0F172A]
[https://img.shields.io/badge/N8N-EA4B71?style=flat-square&logo=n8n&logoColor=white]
[https://img.shields.io/badge/Telegram-26A5E4?style=flat-square&logo=telegram&logoColor=white]

</td>
<td width="50%" valign="top">

### 🌐 Operação de TI, Redes & Estudos
Vivência prática com **VPNs**, **Wireshark**, **VoIP (Yeastar/Linkus)**, **SharePoint** e **TOTVS RH**, além de projeto acadêmico em **Java** e automação em andamento (**ClickUp–Obsidian**).

[https://img.shields.io/badge/tipo-infra%20%26%20estudos-06B6D4?style=flat-square&labelColor=0F172A]
[https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white]
[https://img.shields.io/badge/Java-ED8B00?style=flat-square]

</td>
</tr>
</table>

<br/>

## 🧰 Arsenal Tecnológico

<div align="center">

<img src="https://skillicons.dev/icons?i=py,fastapi,django,c,postgres,mysql,docker,linux,ubuntu,bash,git,github,githubactions,vscode&theme=dark&perline=7" alt="Arsenal Tecnológico de Rafael Maia" />

</div>

<br/>

```mermaid
flowchart TB
    subgraph L1["APLICAÇÃO & APIs"]
        direction LR
        A1["Python"]
        A2["FastAPI"]
        A3["Django"]
        A4["C"]
    end
    subgraph L2["DADOS & PERSISTÊNCIA"]
        direction LR
        B1["PostgreSQL"]
        B2["MySQL"]
        B3["SQLAlchemy Async"]
    end
    subgraph L3["QUALIDADE, CI/CD & SEGURANÇA"]
        direction LR
        C1["Pytest"]
        C2["Docker"]
        C3["GitHub Actions"]
        C4["JWT · OAuth2 · Trivy"]
    end
    subgraph L4["SISTEMAS & REDES"]
        direction LR
        D1["Linux (Zorin / Ubuntu)"]
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
%%{init: {'gitGraph': {'showBranches': false, 'rotateCommitLabel': true}}}%%
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

<img height="165" src="https://github-readme-stats.vercel.app/api?username=rafaelmaia-dev&show_icons=true&locale=pt-br&bg_color=0F172A&title_color=A78BFA&icon_color=38BDF8&text_color=E2E8F0&border_color=312E81&border_radius=10&hide_border=false" alt="Estatísticas do GitHub de Rafael Maia" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=rafaelmaia-dev&layout=compact&langs_count=6&locale=pt-br&bg_color=0F172A&title_color=A78BFA&text_color=E2E8F0&border_color=312E81&border_radius=10&hide_border=false" alt="Linguagens mais usadas por Rafael Maia" />

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
> O jeito mais rápido de falar comigo é pelo **LinkedIn**. Se você é recrutador, tech lead ou dev querendo trocar ideia sobre **vagas de back-end, infraestrutura ou sobre o AgentWire**, só chamar lá.

<div align="center">

[[https://img.shields.io/badge/Chamar%20no%20LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white]](https://www.linkedin.com/in/rafael-maia-508554232)
[[https://img.shields.io/badge/Explorar%20Reposit%C3%B3rios-181717?style=for-the-badge&logo=github&logoColor=white]](https://github.com/rafaelmaia-dev?tab=repositories)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:06B6D4,55:5B21B6,100:0F172A&height=120&section=footer" width="100%" />

</div>
