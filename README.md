<div align="center">

<img src="assets/banner.svg" alt="Rafael Maia, desenvolvedor back-end que sabe onde o código roda" width="100%"/>

<br/>

![Status](https://img.shields.io/badge/status-aberto%20a%20est%C3%A1gio%20ou%20j%C3%BAnior-2ea043?style=flat-square&labelColor=1a1a2e)
![Foco](https://img.shields.io/badge/foco-back--end-7C3AED?style=flat-square&labelColor=1a1a2e)
![Local](https://img.shields.io/badge/local-Brasil-4F46E5?style=flat-square&labelColor=1a1a2e)

[**LinkedIn**](https://www.linkedin.com/in/rafael-maia-508554232) &nbsp;·&nbsp; [**GitHub**](https://github.com/rafaelmaia-dev) &nbsp;·&nbsp; [**AgentWire**](https://github.com/rafaelmaia-dev/bot_noticias_ia)

</div>

<br/>

Se este perfil fosse uma API, a resposta seria esta:

```http
GET /rafael

200 OK
```

```json
{
  "nome": "Rafael Maia",
  "papel": "desenvolvedor back-end em formação",
  "agora": {
    "trabalho": "Auxiliar de Instalação @ Procfit (PDV, pré-venda e VPNs)",
    "estudo": "Sistemas de Informação, FALS (6º semestre, conclusão em dez/2027)",
    "construindo": "AgentWire, um bot que acompanha as novidades dos agentes de IA"
  },
  "stack": ["Python", "FastAPI", "PostgreSQL", "Docker"],
  "diferencial": "vivência em redes, VPNs e instalação de sistemas: sei onde o código roda",
  "procurando": "estágio ou vaga júnior em desenvolvimento back-end"
}
```

<br/>

## 01 · Sobre

Sou estudante de Sistemas de Informação (6º semestre, FALS) e atuo como **Auxiliar de Instalação na Procfit**, no time de instalações de PDV, pré-venda e VPNs. Antes, fui estagiário de Infraestrutura no Instituto Almai. Foi nesses lugares que aprendi a olhar para o outro lado do software: **onde ele é instalado, em que rede ele roda e o que acontece quando algo para de funcionar.**

Agora levo essa base para o back-end. Trabalho com **Python (FastAPI e Django)**, bancos relacionais (**PostgreSQL e MySQL**) e **Docker, Git e GitHub Actions**, e construo o **AgentWire**, um bot que acompanha as novidades dos agentes de IA. Procuro uma oportunidade de **estágio ou vaga júnior em desenvolvimento back-end**.

| Período | Função | Onde | O que faço (ou fiz) |
|---|---|---|---|
| ago/2026 – atual | Auxiliar de Instalação | Procfit | Time de instalações: PDV, pré-venda e VPNs |
| nov/2025 – jul/2026 | Estagiário de Infraestrutura | Instituto Almai | Redes, configuração de ambientes e suporte técnico (N1 e N2) |

<br/>

## 02 · Projeto em destaque: AgentWire

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
    A["🌐 Fontes<br/>RSS · GitHub · HN · Hugging Face"] --> B["🧹 Parser +<br/>Deduplicação"]
    B --> C[("🐘 PostgreSQL")]
    C --> D["🧠 Resumo<br/>Groq API"]
    D --> E["📲 Telegram"]
    C --> F["⚡ API REST<br/>FastAPI"]
    classDef p fill:#7C3AED,stroke:#4F46E5,color:#fff
    classDef db fill:#4F46E5,stroke:#7C3AED,color:#fff
    class A,B,D,E,F p
    class C db
```

<sub>As fontes além de RSS fazem parte do roadmap do projeto.</sub>

<br/>

## 03 · Stack

<table>
  <tr>
    <td><b>Linguagens</b></td>
    <td>
      <img src="assets/icons/python.svg" height="22" alt=""/> Python &nbsp;&nbsp;
      <img src="assets/icons/c.svg" height="22" alt=""/> C
    </td>
  </tr>
  <tr>
    <td><b>Frameworks</b></td>
    <td>
      <img src="assets/icons/fastapi.svg" height="22" alt=""/> FastAPI &nbsp;&nbsp;
      <img src="assets/icons/django.svg" height="22" alt=""/> Django
    </td>
  </tr>
  <tr>
    <td><b>Dados</b></td>
    <td>
      <img src="assets/icons/postgresql.svg" height="22" alt=""/> PostgreSQL &nbsp;&nbsp;
      <img src="assets/icons/mysql.svg" height="22" alt=""/> MySQL
    </td>
  </tr>
  <tr>
    <td><b>DevOps</b></td>
    <td>
      <img src="assets/icons/docker.svg" height="22" alt=""/> Docker &nbsp;&nbsp;
      <img src="assets/icons/git.svg" height="22" alt=""/> Git &nbsp;&nbsp;
      <img src="assets/icons/github.svg" height="22" alt=""/> GitHub &nbsp;&nbsp;
      <img src="assets/icons/githubactions.svg" height="22" alt=""/> GitHub Actions
    </td>
  </tr>
  <tr>
    <td><b>Sistemas e redes</b></td>
    <td>
      <img src="assets/icons/linux.svg" height="22" alt=""/> Linux &nbsp;&nbsp;
      <img src="assets/icons/wireshark.svg" height="22" alt=""/> Wireshark &nbsp;&nbsp;
      VPN &nbsp;&nbsp; Redes de computadores
    </td>
  </tr>
  <tr>
    <td><b>Testes</b></td>
    <td><img src="assets/icons/pytest.svg" height="22" alt=""/> Pytest</td>
  </tr>
  <tr>
    <td><b>Ferramentas de IA</b></td>
    <td>
      <img src="assets/icons/antigravity.svg" height="22" alt=""/> Antigravity &nbsp;&nbsp;
      <img src="assets/icons/githubcopilot.svg" height="22" alt=""/> GitHub Copilot
    </td>
  </tr>
</table>

Aprofundando agora: SQLAlchemy assíncrono e Alembic, testes com Pytest e CI/CD com GitHub Actions.

<br/>

## 04 · Outros projetos

| Projeto | O que faz | Tecnologia |
|---|---|---|
| [**API Google**](https://github.com/rafaelmaia-dev/api-google) | Script com requisição GET via link, simulando a integração com APIs externas | Python |
| [**Calculadora**](https://github.com/rafaelmaia-dev/calculadora-while) | Aplicação de terminal com menu interativo para operações aritméticas, usando `while` | Python |

<br/>

## 05 · Formação

- **FALS** (Faculdade do Litoral Sul Paulista): Sistemas de Informação, 6º semestre, conclusão em dez/2027
- **FastAPI: APIs Modernas e Assíncronas com Python**: Udemy, Geek University, 12,5 horas (concluído em nov/2026)
- **Redes de Computadores com Wireshark** e **Git e GitHub**: Udemy
- **Inglês**: CNA Master in English

<br/>

## 06 · Contato

Recrutadores e tech leads: o caminho mais rápido é o [**LinkedIn**](https://www.linkedin.com/in/rafael-maia-508554232). Também converso sobre back-end, infra e sobre o AgentWire por lá.

<br/>

<div align="center">
<sub>Escrevo código que sabe onde vai rodar.</sub>
</div>
