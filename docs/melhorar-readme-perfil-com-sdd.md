# Melhorando um README de perfil do GitHub com Spec-Driven Development (SDD)

Guia prático para transformar um README de perfil (`usuario/usuario`) em uma **apresentação estratégica de carreira**, usando **Spec-Driven Development**: especificar antes de implementar.

> **A regra de ouro do SDD:** você não escreve o README primeiro. Você escreve a **spec** primeiro. O README é a *implementação* da spec — e a spec é o que você valida contra os critérios de aceite.

---

## Por que SDD (e não só "mexer no markdown")

Editar um README direto no arquivo quase sempre produz o mesmo resultado: uma **parede de logos de tecnologia sem narrativa**. Isso acontece porque não há um alvo definido — cada edição é uma decisão isolada.

O SDD inverte a ordem:

```
Spec  →  Plano  →  Implementação  →  Validação  →  Iteração
 (o quê e por quê)   (como)          (fazer)       (checar contra a spec)
```

Cada fase gera um artefato. A spec vira contrato: se uma seção não atende a spec, ela sai.

---

## Fase 1 — Especificação (o "spec")

Preencha a [spec-template.md](spec-template.md). Os campos essenciais:

### 1.1 Objetivo de posicionamento
Uma frase: **"Quero ser reconhecida como ___."**
Exemplo real deste perfil: *"AI Advocate especializada em Qualidade de Software"*.

### 1.2 Público-alvo
Quem precisa "comprar" esse posicionamento em 10 segundos?
Ex.: recrutadores internacionais, Engineering Managers, Staff Engineers, AI Leaders, CTOs.

### 1.3 Proposta de valor — o teste dos 10 segundos
Escreva o que você quer que a pessoa **pense** ao ler o topo por 10 segundos.
Se hoje ela pensa *"QA que automatiza testes"* e você quer *"lidera transformação de qualidade com IA"*, esse é o **gap** que a spec precisa fechar.

### 1.4 Requisitos
- **Funcionais:** o que o README precisa conter (headline, bio, foco atual, prova social, projetos).
- **Não-funcionais:** bilíngue? responsivo? imagens de fontes estáveis? sem excesso de emoji?

### 1.5 Anti-requisitos (o que evitar)
Igualmente importante. Ex.: *não* parecer QA tradicional; *não* usar "explorando/estudando"; *não* virar lista de logos.

### 1.6 Critérios de aceite
Checklist objetivo e testável. Ex.:
- [ ] Nos primeiros 10s, o leitor identifica "AI + Qualidade", não só "QA".
- [ ] Existe narrativa (não só lista de tecnologias).
- [ ] Verbos de construção, não de aprendiz.
- [ ] PT e EN em paridade total.
- [ ] Nenhuma imagem de fonte frágil; nenhum link quebrado.

---

## Fase 2 — Planejamento

Traduza a spec em **estrutura**, antes de escrever qualquer copy.

### 2.1 Ordem das seções (hierarquia importa)
A ordem comunica prioridade. Se IA é o foco, IA vem **antes** da stack de ferramentas. Exemplo de esqueleto:

```
Headline (posicionamento)  →  Sub-headline (keywords)  →  Bio em prosa
→  🎯 No que estou trabalhando agora  →  🧪 AI Projects
→  🛠️ Tech Stack (suporte, não protagonista)  →  📊 Stats
```

### 2.2 Decisões de design (registre-as)
- **Idioma:** PT, EN, ou bilíngue espelhado com toggle?
- **Layout:** seções espelhadas, intercaladas, ou principal + resumo?
- **Cores:** defina 1 cor de acento e reutilize (evita "arco-íris").

Registrar a decisão evita retrabalho e mantém coerência quando um agente de IA editar depois (veja o [AGENTS.md](../AGENTS.md)).

---

## Fase 3 — Implementação

Agora sim, escreva — **seção por seção, contra a spec**.

- **Headline:** lidere com o posicionamento (o termo que você quer "possuir"), não com o cargo.
- **Bio:** prosa em primeira pessoa. Cases reais > adjetivos. Verbos de construção.
- **Foco atual:** bullets concretos do que você faz *hoje* (com nomes reais: agentes, MCP, guardrails, SDD).
- **Tech Stack:** reduza ao essencial e organize por **capacidade**, não por "quantos logos eu sei".

> Dica de manutenção: se for bilíngue, edite **os dois idiomas na mesma passada** para nunca quebrar o espelho.

---

## Fase 4 — Validação

Rode o README contra os **critérios de aceite** da spec. Três testes rápidos:

1. **Teste dos 10 segundos:** peça a alguém (ou a um LLM) para dizer, em uma frase, o que você faz — lendo só o topo por 10s. Bateu com a proposta de valor? Se não, a headline/bio falharam.
2. **Revisão por persona:** leia como se fosse um recrutador internacional, um Staff Engineer, um AI Leader. A imagem muda conforme a persona? Deveria ser consistente.
3. **Higiene técnica:** links e imagens quebradas? Âncoras funcionam **no GitHub** (não confie no preview do VSCode — veja nota abaixo)? Paridade PT/EN?

### Nota sobre âncoras (uma armadilha comum)
Títulos com emoji geram âncoras diferentes em renderizadores diferentes. O GitHub **mantém** o *variation selector* (U+FE0F) de emojis como `🛠️`. Ex.: `🛠️ Tech Stack` → âncora `#%EF%B8%8F-tech-stack`. Sempre pegue o link real clicando no ícone de âncora do título **no GitHub renderizado**.

---

## Fase 5 — Iteração

A spec é viva. Quando surgir algo novo (um projeto publicado, uma palestra), volte à spec, atualize os requisitos e reimplemente a seção afetada. Nada de edições soltas fora do contrato.

### Automatize a validação (bônus muito on-brand para QA)
Um CI que valida o próprio README — links/imagens quebradas e paridade PT/EN — transforma a Fase 4 em algo contínuo. É *dogfooding* de qualidade no seu próprio perfil.

---

## Resumo em uma linha

**Não edite o README. Especifique-o, planeje-o, implemente-o contra a spec e valide-o.** O markdown é só o último passo.
