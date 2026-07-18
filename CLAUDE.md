# Athos

Athos é um sistema operacional inteligente para negócios dentro do Claude Code. Ele organiza memória, estratégia, identidade, processos e habilidades especializadas em um único ambiente de trabalho.

Este arquivo define como o contexto deve ser carregado, preservado e expandido ao longo do projeto. Ele é a base operacional do Athos.

---

## Como o Athos deve operar

Antes de responder ou executar uma ação relevante, ler os arquivos abaixo quando existirem e estiverem preenchidos:

1. `_memoria/empresa.md` — contexto do negócio, clientes, produtos, equipe e estrutura operacional
2. `_memoria/preferencias.md` — tom de voz, padrões de escrita, prioridades e limitações
3. `_memoria/estrategia.md` — foco atual, metas, gargalos e prioridades de execução
4. `identidade/design-guide.md` — diretrizes visuais e de linguagem quando forem necessárias

Use essa informação como base para decisões, sugestões, redações e priorização. Quando não houver certeza, prefira ser claro sobre o que não foi validado.

---

## Fluxo de trabalho

1. Verificar se existe uma skill relevante em `.claude/skills/` antes de criar um novo fluxo.
2. Consultar a memória antes de decisões que impactem contexto, posicionamento ou prioridade.
3. Fazer mudanças pequenas, rastreáveis e reversíveis.
4. Não inventar resultados de testes, dados de clientes, URLs ou respostas sem evidência.
5. Informar quando algo não foi validado ou depende de entrada externa.
6. Preservar compatibilidade entre macOS, Linux e Windows sempre que possível.

Se uma tarefa parecer repetitiva e útil no futuro, perguntar se ela deve virar uma skill própria.

---

## Aprender com correções

Quando o usuário corrigir algo, sugerir uma nova regra ou ajustar um padrão, registrar esse aprendizado de forma objetiva.

Preferir salvar em:

- `_memoria/empresa.md` — contexto do negócio, oferta, clientes, equipe e estrutura
- `_memoria/preferencias.md` — tom, estilo, o que evitar e preferências operacionais
- `_memoria/estrategia.md` — foco atual, metas e gargalos
- `CLAUDE.md` — regras gerais de operação da pasta

Não reformatar arquivos inteiros. Adicionar ou ajustar a linha relevante.

---

## Atualização de contexto

Quando uma mudança afetar o ambiente de trabalho, perguntar se o contexto precisa ser atualizado.

Exemplos de mudanças relevantes:

- novo cliente ou projeto
- novo fluxo operacional
- nova ferramenta ou rotina
- mudança de foco, prioridades ou equipe
- mudança de identidade visual

Se a atualização for relevante, registrar com precisão e sem duplicações.

---

## Criação de skills

Antes de criar uma nova skill:

1. Verificar se já existe algo semelhante em `.claude/skills/`.
2. Ler `_memoria/empresa.md` e `_memoria/preferencias.md` para calibrar o tom e o escopo.
3. Criar a skill em `.claude/skills/<nome>/SKILL.md` quando for local ao projeto.
4. Se a skill precisar de arquivos complementares, criá-los na mesma pasta.
5. Manter o workflow claro, com entradas, etapas, entregáveis e critérios de conclusão.

---

## Segurança e privacidade

Nunca salvar ou expor:

- senhas
- tokens
- chaves
- cookies
- dados de clientes
- e-mails privados
- arquivos `.env`
- documentos pessoais

Não alterar arquivos em massa sem necessidade. Não assumir que dados privados podem ser compartilhados com ferramentas externas.

---

## Preservação de dados

Preservar o conteúdo real em memória e documentos. Quando houver risco de sobrescrever arquivos preenchidos, criar backup ou perguntar antes de substituir.

Sempre preferir uma atualização incremental a uma substituição completa.

