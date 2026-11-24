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

| Camada | Ferramentas |
|---|---|
| **Linguagens** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![C](https://img.shields.io/badge/C-659AD2?style=flat-square&logo=c&logoColor=white) |
| **Frameworks** | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Django](https://img.shields.io/badge/Django-0C4B33?style=flat-square&logo=django&logoColor=white) |
| **Dados** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) |
| **DevOps** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-3B3F46?style=flat-square&logo=github&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) |
| **Sistemas e redes** | ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) ![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square) ![VPN](https://img.shields.io/badge/VPN-4F46E5?style=flat-square) ![Redes de computadores](https://img.shields.io/badge/Redes%20de%20computadores-4F46E5?style=flat-square) |
| **Testes** | ![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white) |
| **Ferramentas de IA** | ![Antigravity](https://img.shields.io/badge/Antigravity-4285F4?style=flat-square) ![GitHub Copilot](https://img.shields.io/badge/GitHub%20Copilot-8957E5?style=flat-square&logo=githubcopilot&logoColor=white) |

Aprofundando agora: SQLAlchemy assíncrono e Alembic, testes com Pytest e CI/CD com GitHub Actions.

## Outros projetos

| Projeto | O que faz | Tecnologia |
|---|---|---|
| [**API Google**](https://github.com/rafaelmaia-dev/api-google) | Script com requisição GET via link, simulando a integração com APIs externas | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) |
| [**Calculadora**](https://github.com/rafaelmaia-dev/calculadora-while) | Aplicação de terminal com menu interativo para operações aritméticas, usando `while` | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) |

## Formação

<details>
<summary><b>Faculdade e cursos</b></summary>

<br/>

- **FALS** (Faculdade do Litoral Sul Paulista): Sistemas de Informação, 6º semestre, conclusão em dez/2027
- **FastAPI: APIs Modernas e Assíncronas com Python**: Udemy, Geek University, 12,5 horas (concluído em nov/2026)
- **Redes de Computadores com Wireshark** e **Git e GitHub**: Udemy
- **Inglês**: CNA Master in English

</details>

## Contato

Recrutadores e tech leads: o caminho mais rápido é o [**LinkedIn**](https://www.linkedin.com/in/rafael-maia-508554232). Converso por lá sobre back-end, infra e sobre o AgentWire.

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7C3AED,100:4F46E5&height=120&section=footer" width="100%"/>

</div>
