<div align="center">

# ✂️ ClaudeSlim

**Um skill para o Claude Code responder direto, com precisão e sem enrolação.**

![Versão](https://img.shields.io/badge/vers%C3%A3o-2.0-blue)
![Licença](https://img.shields.io/badge/licen%C3%A7a-MIT-green)
![Claude Code](https://img.shields.io/badge/Claude%20Code-skill-orange)

*Cole o link deste repositório no Claude Code e ele instala o skill no seu projeto.*

</div>

> 🇬🇧 **English:** ClaudeSlim is a Claude Code skill (Developer / Professional editions) that makes Claude more direct, accurate and honest. Paste this repo's link into Claude Code and ask it to install it. See [INSTALL.md](INSTALL.md).

---

## 🚀 Instalação em 10 segundos

Abra seu projeto no **Claude Code** e envie:

```text
Instale o ClaudeSlim neste projeto: https://github.com/MiguelHort/claudeslim
```

O Claude lê o [INSTALL.md](INSTALL.md), escolhe a edição certa para o seu projeto e cria o skill em:

```text
.claude/skills/claudeslim/SKILL.md
```

Ele **não altera** seu `CLAUDE.md` nem outros arquivos, e **não faz commit**.

Depois, **reinicie o Claude Code** (ou abra uma nova sessão) no projeto. O Claude Code só encontra skills novos quando a sessão começa.

> Quer escolher a edição? Diga: *"…instale a edição Developer"* ou *"…a edição Professional"*.

---

## 🧭 Qual edição escolher?

| | 💻 **Developer** | 💼 **Professional** |
|---|---|---|
| **Para** | Trabalhar com código | Tarefas profissionais em geral |
| **Ajuda a** | Criar funcionalidades e corrigir bugs, analisar código, logs e erros, revisar implementações, entender a estrutura do projeto | Escrever e revisar textos e e-mails, analisar documentos e dados, pesquisar e comparar alternativas, criar relatórios e apoiar decisões |
| **Arquivo** | [`skills/developer/SKILL.md`](skills/developer/SKILL.md) | [`skills/professional/SKILL.md`](skills/professional/SKILL.md) |

💡 **Dica:** instale **uma** edição por projeto. As duas usam o mesmo nome de skill (`claudeslim`), então a segunda substituiria a primeira.

---

## ✨ O que o ClaudeSlim faz

- 🎯 **Responde o pedido real**: vai direto ao ponto, sem repetir o que já foi dito e sem perguntar o que já está no contexto.
- 🧠 **Economiza contexto sem perder qualidade**: evita ler ou repetir o que não é necessário, mas nunca corta detalhe importante.
- ✅ **Honestidade em primeiro lugar**: não inventa arquivos, APIs, fontes, números nem resultados de teste. Separa fato, suposição e estimativa.
- 🙅 **Sem concordar por educação**: aponta premissas erradas e explica o porquê.
- ✍️ **Escrita clara e controlada**: termos consistentes, frases diretas, passos explícitos. Inspirada em *Simplified Technical English*, sem alegar conformidade com o ASD-STE100.

**Só na edição Developer:** inspeciona o repositório antes de alterar, faz a menor mudança que resolve, depura com evidência, revisa código, nunca diz que um teste passou sem executá-lo e entrega um relatório final (*Implemented / Validation / Not verified*).

**Só na edição Professional:** entende objetivo, público e formato, checa fontes, preserva datas, valores e termos de documentos, separa achados de recomendações e faz um checklist antes de responder.

---

## ✅ Como conferir se funcionou

1. Reinicie o Claude Code no projeto.
2. Digite `/` e procure por **`claudeslim`** na lista.
3. Ou pergunte: *"Quais skills estão disponíveis neste projeto?"*

---

## 🛠️ Instalação manual

Prefere fazer sozinho? Copie o arquivo da edição escolhida para o seu projeto:

```bash
mkdir -p .claude/skills/claudeslim
curl -fsSL https://raw.githubusercontent.com/MiguelHort/claudeslim/main/skills/developer/SKILL.md \
  -o .claude/skills/claudeslim/SKILL.md
```

Para a edição Professional, troque `developer` por `professional` na URL.

**Para todos os seus projetos:** use `~/.claude/skills/claudeslim/SKILL.md` no lugar de `.claude/skills/claudeslim/SKILL.md`.

**Desinstalar:** apague a pasta `.claude/skills/claudeslim/`.

---

## 🚫 O que o ClaudeSlim **não** faz

Seja realista: o skill orienta o **comportamento** do Claude. Ele **não** aumenta cotas, velocidade, limites de uso nem a janela de contexto, e **não** garante uma economia fixa de tokens. O Claude também decide quando carregar um skill com base na descrição dele. Para forçar o uso em uma conversa, digite `/claudeslim`.

---

## 📁 Estrutura

```text
claudeslim/
├── README.md
├── INSTALL.md                  # instruções para o Claude Code instalar o skill
├── skills/
│   ├── developer/SKILL.md      # edição para código
│   └── professional/SKILL.md   # edição para trabalho em geral
├── docs/
│   └── ClaudeSlim_Guia.pptx    # guia rápido em slides
└── LICENSE
```

📊 Prefere slides? Veja o [guia rápido](docs/ClaudeSlim_Guia.pptx).

---

## 🤝 Contribuindo

Sugestões e melhorias são bem-vindas: abra uma *issue* ou um *pull request*. Ao propor uma regra nova, evite duplicar ou contradizer as existentes e não prometa ganhos que não foram medidos.

## 📄 Licença

[MIT](LICENSE)
