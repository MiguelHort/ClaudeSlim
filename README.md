<div align="center">

# ⚡ AI Efficiency Kit

**Regras prontas para sua IA responder direto, com precisão e sem enrolação.**

![Versão](https://img.shields.io/badge/vers%C3%A3o-2.0-blue)
![Licença](https://img.shields.io/badge/licen%C3%A7a-MIT-green)
![Edições](https://img.shields.io/badge/edi%C3%A7%C3%B5es-Developer%20%7C%20Professional-orange)

*Instale em qualquer projeto: cole o link deste repositório no Claude e pronto.*

</div>

> 🇬🇧 **English:** a pair of drop-in rule files (Developer / Professional) that make AI assistants more direct, accurate and honest. Paste this repo's link into Claude Code and ask it to install the kit. See [INSTALL.md](INSTALL.md).

---

## 🚀 Instalação em 10 segundos

Abra seu projeto no **Claude Code** (ou outro agente de IA) e envie:

```text
Instale o AI Efficiency Kit neste projeto: https://github.com/MiguelHort/ai-efficiency-kit
```

O agente lê o [INSTALL.md](INSTALL.md), escolhe a edição certa para o seu projeto, adiciona as regras no lugar que a sua ferramenta reconhece e mostra o que mudou. Ele **não faz commit** nem sobrescreve suas instruções existentes.

> Quer escolher a edição? Diga: *"…instale a edição Developer"* ou *"…a edição Professional"*.

---

## 🧭 Qual edição escolher?

| | 💻 **Developer** | 💼 **Professional** |
|---|---|---|
| **Para** | Trabalhar com código | Tarefas profissionais em geral |
| **Ajuda a** | Criar funcionalidades e corrigir bugs, analisar código, logs e erros, revisar implementações, entender a estrutura do projeto | Escrever e revisar textos e e-mails, analisar documentos e dados, pesquisar e comparar alternativas, criar relatórios e apoiar decisões |
| **Ferramentas** | Claude Code, Codex, Cursor, Copilot, Gemini CLI | Claude, ChatGPT e outros assistentes com instruções personalizadas |
| **Arquivo** | [`AI-EFFICIENCY-DEVELOPER.md`](rules/AI-EFFICIENCY-DEVELOPER.md) | [`AI-EFFICIENCY-PROFESSIONAL.md`](rules/AI-EFFICIENCY-PROFESSIONAL.md) |

💡 **Dica:** instale **uma** edição por ambiente. Carregar as duas sem necessidade só duplica instruções.

---

## ✨ O que o kit faz

- 🎯 **Responde o pedido real**: vai direto ao ponto, sem repetir o que já foi dito e sem perguntar o que já está no contexto.
- 🧠 **Economiza contexto sem perder qualidade**: evita ler ou repetir o que não é necessário, mas nunca corta detalhe importante.
- ✅ **Honestidade em primeiro lugar**: não inventa arquivos, APIs, fontes, números nem resultados de teste. Separa fato, suposição e estimativa.
- 🙅 **Sem concordar por educação**: aponta premissas erradas e explica o porquê.
- ✍️ **Escrita clara e controlada**: termos consistentes, frases diretas, passos explícitos. Inspirada em *Simplified Technical English*, sem alegar conformidade com o ASD-STE100.

**Só na edição Developer:** inspeciona o repositório antes de alterar, faz a menor mudança que resolve, depura com evidência, revisa código, nunca diz que um teste passou sem executá-lo e entrega um relatório final (*Implemented / Validation / Not verified*).

**Só na edição Professional:** entende objetivo, público e formato, checa fontes, preserva datas, valores e termos de documentos, separa achados de recomendações e faz um checklist antes de responder.

---

## 🛠️ Instalação manual

Prefere fazer sozinho? Copie a edição escolhida para o lugar que a sua ferramenta lê:

| Ferramenta | Onde colocar |
|---|---|
| **Claude Code** | Copie para `.claude/ai-efficiency.md` e adicione `@.claude/ai-efficiency.md` ao `CLAUDE.md` |
| **Codex e outras ferramentas com `AGENTS.md`** | Cole o conteúdo no `AGENTS.md` |
| **Cursor** | `.cursor/rules/ai-efficiency.mdc` (com `alwaysApply: true`) |
| **GitHub Copilot** | `.github/copilot-instructions.md` |
| **Gemini CLI** | `GEMINI.md` |
| **Claude.ai, ChatGPT e similares** | Cole nas instruções do projeto ou nas instruções personalizadas |

Detalhes e como desinstalar: [INSTALL.md](INSTALL.md).

> ⚠️ Não basta salvar o `.md` em qualquer pasta. A ferramenta precisa reconhecer aquele local ou mecanismo de instruções. Depois de instalar, abra uma **nova sessão** para as regras carregarem.

---

## ✅ Como testar se funcionou

1. Abra uma nova sessão na ferramenta.
2. Peça algo simples, por exemplo: *"Quais regras de trabalho você está seguindo neste projeto?"*
3. Confira se ela menciona as regras do AI Efficiency Kit.

---

## 🚫 O que o kit **não** faz

Seja realista: as instruções orientam o **comportamento** da IA. Elas **não** aumentam cotas, velocidade, limites de uso nem a janela de contexto, e **não** garantem uma economia fixa de tokens.

---

## 📁 Estrutura

```text
ai-efficiency-kit/
├── README.md
├── INSTALL.md                          # instruções para o agente de IA instalar o kit
├── rules/
│   ├── AI-EFFICIENCY-DEVELOPER.md      # edição para código
│   └── AI-EFFICIENCY-PROFESSIONAL.md   # edição para trabalho em geral
├── docs/
│   └── AI_Efficiency_Kit_Guia.pptx     # guia rápido em slides
└── LICENSE
```

📊 Prefere slides? Veja o [guia rápido](docs/AI_Efficiency_Kit_Guia.pptx).

---

## 🤝 Contribuindo

Sugestões e melhorias são bem-vindas: abra uma *issue* ou um *pull request*. Ao propor uma regra nova, evite duplicar ou contradizer as existentes e não prometa ganhos que não foram medidos.

## 📄 Licença

[MIT](LICENSE)
