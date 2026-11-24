<div align="center">

<img width="100%" alt="Rafael Maia" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=200&section=header&text=Rafael%20Maia&fontSize=80&fontColor=fff&animation=twinkling&fontAlignY=35&desc=Back-end%20que%20sabe%20onde%20o%20c%C3%B3digo%20roda&descAlignY=60&descSize=22&descColor=c0c0ff" />

![Status](https://img.shields.io/badge/status-aberto%20a%20est%C3%A1gio%20ou%20j%C3%BAnior-2ea043?style=flat-square&labelColor=1a1a2e)
![Foco](https://img.shields.io/badge/foco-back--end-7C3AED?style=flat-square&labelColor=1a1a2e)
![Local](https://img.shields.io/badge/local-Brasil-4F46E5?style=flat-square&labelColor=1a1a2e)

[LinkedIn](https://www.linkedin.com/in/rafael-maia-508554232) · [GitHub](https://github.com/rafaelmaia-dev) · [AgentWire](https://github.com/rafaelmaia-dev/bot_noticias_ia)

</div>

```bash
$ systemctl status rafael

● rafael.service - desenvolvedor back-end em formação
     Loaded: loaded (FALS · Sistemas de Informação · 6º sem. · dez/2027)
     Active: active (running) · aberto a estágio ou vaga júnior
   Main PID: Procfit · Auxiliar de Instalação (PDV, pré-venda e VPNs)
      Tasks: 1 em desenvolvimento (AgentWire)
     Memory: Python · FastAPI · PostgreSQL · Docker
```

## Sobre

Sou estudante de Sistemas de Informação (6º semestre, FALS) e atuo como **Auxiliar de Instalação na Procfit**, no time de instalações de PDV, pré-venda e VPNs. Antes, fui estagiário de Infraestrutura no Instituto Almai. Foi nesses lugares que aprendi a olhar para o outro lado do software: **onde ele é instalado, em que rede ele roda e o que acontece quando algo para de funcionar.**

Agora levo essa base para o back-end. Trabalho com **Python (FastAPI e Django)**, bancos relacionais (**PostgreSQL e MySQL**) e **Docker, Git e GitHub Actions**, e construo o **AgentWire**, um bot que acompanha as novidades dos agentes de IA.

> [!IMPORTANT]
> **Aberto a oportunidades:** busco estágio ou vaga júnior em desenvolvimento back-end.

## Do cabo ao código

Meu caminho, no formato que eu mais gosto de ler: um `git log`.

```mermaid
%%{init: {'gitGraph': {'showBranches': false, 'rotateCommitLabel': true}}}%%
gitGraph
    commit id: "FALS"
    commit id: "Almai: infra e redes"
    branch back-end
    checkout back-end
    commit id: "Python e FastAPI"
    commit id: "AgentWire"
    checkout main
    commit id: "Procfit: instalações e VPNs"
    checkout back-end
    commit id: "Curso de FastAPI"
    commit id: "próximo: vaga júnior" type: HIGHLIGHT
```

## Projeto em destaque: AgentWire

> Bot no Telegram que mantém devs e vibe coders por dentro das novidades dos agentes de IA.

![Status](https://img.shields.io/badge/status-em%20desenvolvimento-F59E0B?style=flat-square&labelColor=1a1a2e)
![Último commit](https://img.shields.io/github/last-commit/rafaelmaia-dev/bot_noticias_ia?style=flat-square&label=%C3%BAltimo%20commit&labelColor=1a1a2e&color=4F46E5)
[![Repositório](https://img.shields.io/badge/ver%20o%20reposit%C3%B3rio-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/rafaelmaia-dev/bot_noticias_ia)

**O problema:** as novidades dos agentes de código (Claude Code, Codex, DeepSeek e outros) saem em blogs, repositórios e redes sociais, e acompanhar tudo toma tempo. O AgentWire coleta, resume e entrega no Telegram, com o link da fonte.

- **Pipeline determinístico.** Cada etapa tem entrada e saída bem definidas, e o LLM é usado só para resumir. Não é um agente de IA: é um sistema auditável *sobre* agentes.
- **API REST (FastAPI) e worker separados**, sobre o mesmo PostgreSQL.
- **Testes automatizados e de regressão**, e Docker para rodar na sua própria máquina.
- Desenvolvido com apoio do Antigravity.

```mermaid
flowchart LR
    A["Fontes<br/>RSS · GitHub · HN · Hugging Face"] --> B["Parser +<br/>Deduplicação"]
    B --> C[("PostgreSQL")]
    C --> D["Resumo<br/>Groq API"]
    D --> E["Telegram"]
    C --> F["API REST<br/>FastAPI"]
    classDef p fill:#7C3AED,stroke:#4F46E5,color:#fff
    classDef db fill:#4F46E5,stroke:#7C3AED,color:#fff
    class A,B,D,E,F p
    class C db
```

<sub>As fontes além de RSS fazem parte do roadmap do projeto.</sub>

## Stack

Do app até a rede: as camadas por onde o meu código passa.

```mermaid
flowchart TB
    subgraph L1["APLICAÇÃO"]
        direction LR
        A1["Python"]
        A2["FastAPI"]
        A3["Django"]
        A4["C"]
    end
    subgraph L2["DADOS"]
        direction LR
        B1["PostgreSQL"]
        B2["MySQL"]
    end
    subgraph L3["QUALIDADE E ENTREGA"]
        direction LR
        C1["Pytest"]
        C2["Docker"]
        C3["Git e GitHub"]
        C4["GitHub Actions"]
    end
    subgraph L4["SISTEMAS E REDES"]
        direction LR
        D1["Linux"]
        D2["VPN"]
        D3["Wireshark"]
        D4["Redes"]
    end
    A1 ~~~ A2 ~~~ A3 ~~~ A4
    B1 ~~~ B2
    C1 ~~~ C2 ~~~ C3 ~~~ C4
    D1 ~~~ D2 ~~~ D3 ~~~ D4
    L1 ~~~ L2
    L2 ~~~ L3
    L3 ~~~ L4
    classDef a fill:#7C3AED,stroke:#A855F7,color:#fff,stroke-width:1px
    classDef d fill:#6366F1,stroke:#818CF8,color:#fff,stroke-width:1px
    classDef o fill:#4F46E5,stroke:#6366F1,color:#fff,stroke-width:1px
    classDef i fill:#3730A3,stroke:#4F46E5,color:#fff,stroke-width:1px
    class A1,A2,A3,A4 a
    class B1,B2 d
    class C1,C2,C3,C4 o
    class D1,D2,D3,D4 i
    style L1 fill:#1E1B4B,stroke:#7C3AED,stroke-width:2px,color:#C4B5FD
    style L2 fill:#1E1B4B,stroke:#6366F1,stroke-width:2px,color:#C7D2FE
    style L3 fill:#1E1B4B,stroke:#4F46E5,stroke-width:2px,color:#C7D2FE
    style L4 fill:#1E1B4B,stroke:#3730A3,stroke-width:2px,color:#C7D2FE
```

Desenvolvo com apoio do **Antigravity** e do **GitHub Copilot**.

## Aprofundando agora

- [x] Curso de FastAPI: APIs Modernas e Assíncronas com Python (nov/2026)
- [ ] SQLAlchemy assíncrono e Alembic
- [ ] Testes automatizados e de regressão com Pytest
- [ ] CI/CD com GitHub Actions
- [ ] Concluir o pipeline principal do AgentWire

## Outros projetos

| 🔌 **API Google** | 🧮 **Calculadora** |
|:---|:---|
| Script em Python que faz requisições HTTP (GET) para simular o consumo e o tratamento de respostas de APIs externas.<br><br>![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)<br><br>**Conceitos:** REST, HTTP e respostas de APIs<br><br>[Ver no GitHub →](https://github.com/rafaelmaia-dev/api-google) | Aplicação de terminal com menu interativo para operações matemáticas, com laços `while` para validação e controle de fluxo.<br><br>![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)<br><br>**Conceitos:** lógica de programação e validação de entrada<br><br>[Ver no GitHub →](https://github.com/rafaelmaia-dev/calculadora-while) |

## Formação

| Formação | Onde | Situação |
|:---|:---|:---|
| **Sistemas de Informação** | FALS · Faculdade do Litoral Sul Paulista | ![em andamento](https://img.shields.io/badge/em%20andamento-F59E0B?style=flat-square) 6º semestre · dez/2027 |
| **FastAPI: APIs Modernas e Assíncronas com Python** | Udemy · Geek University · 12,5 h | ![concluído](https://img.shields.io/badge/conclu%C3%ADdo-2ea043?style=flat-square) nov/2026 |
| **Redes de Computadores com Wireshark** | Udemy | curso extra |
| **Git e GitHub** | Udemy | curso extra |
| **Inglês** | CNA Master in English | curso de idioma |

## Contato

> [!TIP]
> O jeito mais rápido de falar comigo é o LinkedIn. Se você é recrutador ou tech lead, me chame para conversar sobre vagas de back-end, infra ou sobre o AgentWire.

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rafael-maia-508554232) [![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/rafaelmaia-dev)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7C3AED,100:4F46E5&height=120&section=footer" width="100%"/>

</div>
