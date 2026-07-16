# AGENTS.md

Instruções para agentes de IA (Claude Code, Devin, Cursor, Copilot, etc.) que forem editar este repositório.

## Contexto do repositório

Este é o **repositório de perfil do GitHub** de `jussaragranja` (o nome do repo é igual ao usuário).
Por isso, o [README.md](README.md) é renderizado automaticamente na página inicial do perfil.

**Objetivo de posicionamento:** apresentar a Ju como **AI Advocate for Software Quality** — não como QA Automation tradicional. Todo texto e estrutura devem reforçar: IA aplicada à qualidade, agentes, LLMs, Software Quality Engineering, AI-native QA.

O processo de melhoria deste README segue **Spec-Driven Development (SDD)** — veja [docs/](docs/).

## Regras ao editar o README

1. **Espelho bilíngue (PT/EN) obrigatório.** O README tem duas seções espelhadas: `## 🇧🇷 Português` e `## 🇬🇧 English`, com o **mesmo conteúdo**. Qualquer alteração em um idioma **deve ser replicada** no outro. Nunca deixe os blocos fora de sincronia.

2. **A seção `## 🛠️ Tech Stack` e tudo abaixo dela é território da autora.** Não reestruture, não remova e não reordene esse bloco (Tech Stack, Estatísticas & Snake, Easter Egg) sem pedir confirmação explícita.

3. **Âncoras seguem o algoritmo do GitHub, não o do preview do VSCode.** O GitHub **mantém** o *variation selector* (U+FE0F) dos emojis nas âncoras. Ex.: o título `🛠️ Tech Stack` gera a âncora `#%EF%B8%8F-tech-stack` (e **não** `#-tech-stack`). Sempre valide âncoras contra o GitHub renderizado — o preview do VSCode usa outro algoritmo e não é fonte de verdade.

4. **Imagens: só fontes estáveis.** Prefira `cdn.jsdelivr.net` (devicon), `img.shields.io`, `simple-icons`. **Evite** hotlink de Pinterest, Medium, blogs, `iconape`, `freelogopng` e afins — quebram com o tempo (e um README de QA com imagem quebrada é péssima imagem).

5. **Cores de badge:** hex de 6 dígitos. O acento da marca é o laranja `F7A41D` (mesmo do typing SVG). Não introduza cores novas sem necessidade.

6. **Tom:** bio em prosa, primeira pessoa, verbos de construção ("construo", "aplico", "crio") — evite "explorando/estudando". Sem excesso de emojis em listas de bio.

7. **Seções ocultas:** `🧪 AI Projects & Labs` está dentro de comentário HTML até haver projetos publicados. Para reativar, remova os marcadores `<!-- ... -->` (em PT e EN).

## Regras de Git

- **Não faça commit nem push sem pedido explícito** da autora.
- Mensagens de commit em português; encerre com o trailer `Co-Authored-By:` quando aplicável.
- Este é um repo pessoal de perfil — o fluxo simples (branch → PR → `master`) é aceitável.

## Onde as coisas moram

- **Config/manutenção deste repo** (este `AGENTS.md`, workflows, docs) → aqui.
- **Cases de portfólio** (agentes, skills, geradores de teste) → **repositórios próprios**, fixados no perfil e linkados em `AI Projects & Labs`. **Não** guarde código de projeto neste repo.
