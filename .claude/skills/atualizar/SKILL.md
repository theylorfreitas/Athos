---
name: atualizar
description: >
  Varre o projeto e atualiza a memória operacional do Athos sem destruir contexto útil. Use quando o usuário disser "atualiza", "/atualizar", "varre o projeto" ou pedir uma reconciliação geral.
---

# /atualizar — Varredura e atualização de contexto

Compara o que está nos arquivos de contexto com o estado real do workspace e propõe atualizações de forma incremental.

## Workflow

### Passo 1 — Levantamento

Listar:
- pastas na raiz
- skills em `.claude/skills/`
- arquivos relevantes de contexto em `_memoria/` e `identidade/`
- mudanças recentes em workspaces ou projetos relevantes

### Passo 2 — Comparação

Ler os arquivos de contexto e identificar:

- **Em `_memoria/empresa.md`:** o contexto operacional ainda bate com a realidade do workspace?
- **Em `_memoria/estrategia.md`:** prioridades e gargalos ainda fazem sentido?
- **Em `CLAUDE.md`:** as regras gerais ainda correspondem ao que existe?
- **Em `identidade/design-guide.md`:** o padrão visual continua coerente?

### Passo 3 — Proposta de mudanças

Apresentar uma lista curta e objetiva, por exemplo:

```text
Encontrei 2 pontos para atualizar:

1. _memoria/empresa.md — falta a equipe ou o perfil operacional atual.
2. _memoria/estrategia.md — a prioridade principal mudou.

Quer que eu aplique essas mudanças?
```

### Passo 4 — Aplicação

Se o usuário aprovar, editar os arquivos com cirurgia — só a linha relevante, sem reformatar o documento todo. Mostrar o que mudou.

## Regras

- Não inventar fatos sem evidência.
- Não apagar conteúdo útil; apenas atualizar ou complementar.
- Evitar duplicações.
- Manter histórico de decisões quando fizer sentido.
- Se nenhuma mudança for necessária, responder que tudo está coerente.
