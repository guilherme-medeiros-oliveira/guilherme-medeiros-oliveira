<!--
  README do perfil (repositório guilherme-medeiros-oliveira/guilherme-medeiros-oliveira).
  Suba na raiz do repositório: README.md, banner.svg e guilherme-medeiros.png.
-->

<div align="center">

<img src="banner.svg" alt="Guilherme Medeiros Oliveira: estudante de Análise e Desenvolvimento de Sistemas, em busca da primeira vaga de Help Desk N1 e criador do NEXUS HelpDesk" width="100%">

<br>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Conectar-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/guilherme-medeiros-oliveira-478b45291)
[![E-mail](https://img.shields.io/badge/E--mail-Falar_comigo-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:medeiros.oliveira.guilherme@gmail.com)
[![NEXUS ao vivo](https://img.shields.io/badge/NEXUS-Testar_ao_vivo-3b82f6?style=for-the-badge&logo=vercel&logoColor=white)](https://helpdesk-nexus-lac.vercel.app)

<!--
  Quando seu portfólio estiver online, remova as marcas de comentário desta linha e troque a URL:
  [![Portfólio](https://img.shields.io/badge/Portf%C3%B3lio-Ver_site-8b5cf6?style=for-the-badge&logo=googlechrome&logoColor=white)](https://SEU-LINK-AQUI)
-->

</div>

---

## 👋 Olá, meu nome é Guilherme

<img align="right" width="150" src="guilherme-medeiros.png" alt="Foto de Guilherme Medeiros Oliveira">

Sou **estudante de Análise e Desenvolvimento de Sistemas** e estou em busca da minha **primeira oportunidade em Help Desk / Suporte N1**, com muita vontade de crescer até o N2.

Gosto de entender o problema de verdade, explicar a solução sem jargão e aprender com cada chamado. Para não esperar a oportunidade chegar, **construí do zero o meu próprio sistema de chamados, o NEXUS**: foi a forma que encontrei de aprender o atendimento por dentro, do protocolo ao chat, do cliente ao técnico.

- 🎯 **Objetivo:** vaga de Help Desk / Suporte N1 (e evoluir para N2)
- 🛠️ **Projeto principal:** NEXUS HelpDesk, no ar e com código aberto
- 🔁 **Rotina:** estudar, construir e documentar (mais de 100 commits só no NEXUS)

---

## 🚀 Projeto em destaque: NEXUS HelpDesk System

<div align="center">

<a href="https://helpdesk-nexus-lac.vercel.app"><img src="https://github.com/guilherme-medeiros-oliveira/helpdesk-nexus/raw/main/logo-nexus.png" alt="Logo do NEXUS HelpDesk" width="120"></a>

**“Ponto de conexão entre o problema e a solução.”**

[![Commits](https://img.shields.io/github/commit-activity/t/guilherme-medeiros-oliveira/helpdesk-nexus?style=flat-square&label=commits&color=3b82f6)](https://github.com/guilherme-medeiros-oliveira/helpdesk-nexus/commits/main)
[![Último commit](https://img.shields.io/github/last-commit/guilherme-medeiros-oliveira/helpdesk-nexus?style=flat-square&label=%C3%BAltimo%20commit&color=22c55e)](https://github.com/guilherme-medeiros-oliveira/helpdesk-nexus/commits/main)
[![Código](https://img.shields.io/badge/c%C3%B3digo-no_GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/guilherme-medeiros-oliveira/helpdesk-nexus)

</div>

> O NEXUS **substitui planilha e WhatsApp**: o cliente abre o chamado, o técnico responde e atualiza o status, e tudo fica registrado com protocolo e histórico.
>
> 💡 *NEXUS vem do latim: o ponto central onde tudo se conecta. Aqui, é o elo entre o problema do usuário e a solução técnica.*

### 🔄 O caminho de um chamado

```mermaid
sequenceDiagram
    autonumber
    actor Cliente as 👤 Cliente
    participant NEXUS as 🎫 NEXUS
    actor Tecnico as 🛠️ Técnico (Admin)
    Cliente->>NEXUS: Abre o chamado (categoria e prioridade)
    NEXUS-->>Cliente: Protocolo NX-000001 · status Aberto
    Tecnico->>NEXUS: Vê todos os chamados no painel
    Tecnico->>NEXUS: Muda o status para Em Andamento
    Cliente->>NEXUS: Mensagem no chat do chamado
    NEXUS-->>Tecnico: Mensagem aparece em até 2 segundos
    Tecnico->>NEXUS: Responde com a solução
    Tecnico->>NEXUS: Fecha o chamado (Fechado)
```

### ✨ O que o sistema faz

| | Recurso | Como funciona |
|:-:|---|---|
| 🎫 | **Protocolo automático** | Cada chamado ganha um número único: `NX-000001`, `NX-000002`… |
| 🗂️ | **Categorias e prioridade** | Suporte Técnico, Rede, Software, Hardware, E-mail e Impressora · 🟢 Baixa 🟡 Média 🔴 Alta |
| 🔄 | **Status do chamado** | Aberto → Em Andamento → Fechado, atualizado pelo técnico |
| 💬 | **Chat dentro do chamado** | Conversa estilo WhatsApp, com histórico salvo e atualização a cada 2 segundos |
| 👥 | **Painéis por perfil** | O cliente vê só os próprios chamados; o admin vê tudo, responde, muda o status e exclui (com confirmação) |
| ⏱️ | **SLA de 4h úteis** | Prazo de atendimento informado ao cliente no sistema |
| 🔐 | **Segurança** | Senhas com `password_hash`, *prepared statements*, saída escapada contra XSS e cookies de sessão `httponly` e `secure` |
| ⚖️ | **LGPD** | Termos de Uso e Política de Privacidade, com aceite antes do login |
| 🕐 | **Horário de Brasília** | Fuso `America/Sao_Paulo` em todo o sistema |
| 📱 | **Responsivo** | Layout adaptável (Flex e Grid) para celular e desktop |

### 📸 Telas

<table>
<tr>
<td align="center" width="50%">
<a href="https://helpdesk-nexus-lac.vercel.app"><img src="https://github.com/guilherme-medeiros-oliveira/helpdesk-nexus/raw/main/dashboard_cliente.png" alt="Painel do cliente no NEXUS, com conversa estilo WhatsApp"></a>
<br><sub><b>Painel do cliente</b> · conversa estilo WhatsApp</sub>
</td>
<td align="center" width="50%">
<a href="https://helpdesk-nexus-lac.vercel.app"><img src="https://github.com/guilherme-medeiros-oliveira/helpdesk-nexus/raw/main/dashboard_admin.png" alt="Painel do admin no NEXUS, com edição e exclusão de chamados"></a>
<br><sub><b>Painel admin</b> · edição e exclusão do chamado</sub>
</td>
</tr>
</table>

### 🧪 Teste em 1 minuto

1. Abra o [NEXUS ao vivo](https://helpdesk-nexus-lac.vercel.app) e crie uma conta (ou use as [contas de teste](https://github.com/guilherme-medeiros-oliveira/helpdesk-nexus#-acesso-de-teste) do projeto).
2. Abra um chamado escolhendo categoria e prioridade.
3. Entre como admin, responda no chat e mude o status.
4. Volte como cliente e veja a resposta chegar.

### 🗺️ Próximos passos: o ecossistema NEXUS

| Módulo | Código | O que vai fazer | Situação |
|---|---|---|---|
| **NEXUS HelpDesk** | `NX-000001` | Gestão de chamados com chat, status e SLA | ✅ No ar |
| **NEXUS Inventory** | `AST-0001` | Controle de ativos com QR Code, nº de série, nota fiscal, usuário responsável e alerta de licença | 🗓️ Planejado |
| **NEXUS KB** | `KB-0001` | Base de conhecimento com busca e avaliação 👍/👎 (editor TinyMCE) | 🗓️ Planejado |
| **NEXUS Check** | — | Monitor de uptime estilo página de status, verificando a cada 5 minutos (cURL + Cron) | 🗓️ Planejado |

---

## 🎧 Como eu atendo um chamado

| 1️⃣ Escutar | 2️⃣ Diagnosticar | 3️⃣ Resolver | 4️⃣ Documentar |
|:---:|:---:|:---:|:---:|
| Entendo o problema com calma e empatia, sem jargão | Faço as perguntas certas e isolo a causa | Aplico a solução, confirmo com o usuário e escalo quando preciso | Registro tudo para o próximo chamado ser mais rápido |

## 🌱 Em estudo e prática

<!-- Ajuste esta lista para refletir exatamente o que você estuda e já sabe fazer. -->
`Windows 10/11` · `Active Directory` · `Redes (TCP/IP, DNS, DHCP)` · `Linux básico` · `Hardware` · `Microsoft 365` · `Acesso remoto` · `Fundamentos de ITIL`

## 💻 Tecnologias

![PHP](https://img.shields.io/badge/PHP-8.2-777BB4?style=flat-square&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8-4479A1?style=flat-square&logo=mysql&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

<details>
<summary><b>📈 Estatísticas do GitHub</b></summary>

<br>

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=guilherme-medeiros-oliveira&show_icons=true&theme=tokyonight&hide_border=true" alt="Estatísticas do GitHub de Guilherme Medeiros Oliveira">
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=guilherme-medeiros-oliveira&layout=compact&theme=tokyonight&hide_border=true" alt="Linguagens mais usadas por Guilherme Medeiros Oliveira">

</div>

</details>

---

## 📫 Vamos conversar?

Estou pronto para começar e aprender rápido. Se você tem uma vaga de **Help Desk / Suporte N1**, ou só quer trocar uma ideia sobre o NEXUS, me chame:

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Conectar-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/guilherme-medeiros-oliveira-478b45291)
[![E-mail](https://img.shields.io/badge/E--mail-Falar_comigo-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:medeiros.oliveira.guilherme@gmail.com)

<br>

**NEXUS HelpDesk** · *Ponto de conexão entre o problema e a solução* 🎧

Gostou do projeto? Deixe uma ⭐ no [repositório do NEXUS](https://github.com/guilherme-medeiros-oliveira/helpdesk-nexus)!

</div>
