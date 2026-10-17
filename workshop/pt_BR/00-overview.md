<!-- l10n-sync: source-file="workshop/00-overview.md" -->
# 🎮 Mona Mayhem — Workshop de GitHub Copilot

---

> **Duração:** ~1 hora  
> **Nível:** Intermediário  
> **Stack:** Astro / Node.js / TypeScript

Crie um aplicativo retrô de fliperama para comparar contribuições do GitHub — **Mona Mayhem** — enquanto aprende todo o espectro de fluxos de trabalho do GitHub Copilot. O workshop oferece **duas trilhas**: uma experiência com VS Code e outra com GitHub Copilot CLI.

---

## 🎯 Escolha sua trilha

- **Trilha do VS Code** — fique no editor e pratique Chat, Plan Mode, Agent Mode, agentes em segundo plano e o ciclo de revisão integrado.
- **Trilha do CLI** — fique no terminal e pratique `copilot`, contexto com `@file`, `/plan`, edições autônomas, `/fleet`, `/delegate` e `/review`.

Siga a trilha que melhor corresponde ao seu fluxo de trabalho.

---

## 📋 Lista de verificação rápida

Antes de começar, confirme:

- [ ] O GitHub Copilot está habilitado para sua conta
- [ ] Node.js instalado
- [ ] Git instalado e configurado
- [ ] Seu navegador e terminal estão prontos

<!-- track:vscode:start -->
- [ ] VS Code **v1.107+** (sem atualizações pendentes)
- [ ] Sessão iniciada na extensão do **GitHub Copilot**
- [ ] Painel do Chat aberto e Agent pronto
<!-- track:vscode:end -->

<!-- track:cli:start -->
- [ ] GitHub Copilot CLI instalado e disponível como `copilot`
- [ ] Autenticado no CLI com `/login`
- [ ] Familiaridade com comandos slash, como `/help`, `/plan` e `/review`
<!-- track:cli:end -->

> 💡 **Dica:** Use o DevContainer para ter um ambiente pré-configurado e começar rapidamente no VS Code.

---

## 🧠 O que você vai aprender

| # | Habilidade | Descrição |
|---|------------|-----------|
| 1 | **Engenharia de contexto** | Ensine ao Copilot sobre sua base de código com instruções, referências e restrições claras |
| 2 | **Planeje primeiro** | Esboce a arquitetura antes da implementação |
| 3 | **Implementação agêntica** | Deixe o Copilot realizar tarefas de codificação em várias etapas, sob sua supervisão |
| 4 | **Design iterativo** | Use o Copilot para transformar o visual e refinar os detalhes de interação |
| 5 | **Fluxos de trabalho paralelos** | Divida o trabalho entre agentes, sessões ou tarefas delegadas |

<!-- track:vscode:start -->
### Foco nos recursos do VS Code

- **Chat + modo Ask** para exploração
- **Plan Mode** para prompts de arquitetura e design
- **Agent Mode** para implementação em vários arquivos
- **Agentes em segundo plano e na nuvem** para polimento em paralelo
<!-- track:vscode:end -->

<!-- track:cli:start -->
### Foco nos recursos do Copilot CLI

- **Sessões interativas do CLI** com `copilot`
- **`/plan` e Shift+Tab** para planejamento estruturado
- **Edições autônomas** com aprovações inline e `/diff`
- **`/fleet`, `/delegate` e `/review`** para paralelismo e etapas de controle de qualidade
<!-- track:cli:end -->

---

## 📚 Partes do laboratório

| Parte | Título | Descrição |
|------|-------|-----------|
| [**01**](01-setup.md) | Configuração e engenharia de contexto | Crie seu repositório, prepare o ambiente e forneça o contexto adequado ao Copilot |
| [**02**](02-plan-and-scaffold.md) | Planejamento e estrutura inicial | Projete a API e a arquitetura da página antes de implementar |
| [**03**](03-agent-mode.md) | Crie o jogo | Conecte a página de batalha e os gráficos de contribuições com ajuda agêntica |
| [**04**](04-design-vibes.md) | Tema orientado pelo design | Transforme a estrutura inicial em uma experiência retrô de fliperama |
| [**05**](05-polish.md) | Polimento e trabalho paralelo | Use fluxos de trabalho com vários agentes para melhorar a UX, a resiliência e a qualidade |
| [**06**](06-bonus.md) | Bônus e extensões | Explore funcionalidades abertas, fluxos de compartilhamento e experimentos extras |

---

## 💡 Dicas profissionais

1. **Mantenha o navegador aberto** — acompanhe as atualizações ao vivo enquanto programa.
2. **Faça commits com frequência** — salve pontos de controle estáveis durante as iterações.
3. **Refine o plano antes de implementar** — planos melhores levam a resultados melhores.
4. **Revise as alterações do Copilot** — use a visualização de diff ou as ferramentas de revisão do CLI em vez de aceitar tudo sem conferir.

<!-- track:vscode:start -->
5. **Use pontos de controle e Desfazer** no chat se uma iteração sair do rumo.
<!-- track:vscode:end -->

<!-- track:cli:start -->
5. **Use `/session`, `/context` e `/share file`** para inspecionar ou preservar seu trabalho.
<!-- track:cli:end -->
