---
name: salvar
description: >
  Salva o trabalho do Athos localmente e publica somente quando o remoto estiver configurado corretamente. Use quando o usuário disser "salvar", "commit", "push", "/salvar" ou pedir backup do trabalho.
---

# /salvar — Salvar no GitHub

Skill de uma função só: garantir que o trabalho do usuário esteja seguro e versionado, sem publicar acidentalmente em um repositório antigo.

## Workflow

### 1. Verificar estado do git

Rodar `git status --short --branch` e `git remote -v`.

- Se não houver repositório Git inicializado, criar um commit inicial local e perguntar se o usuário quer configurar um remote novo.
- Se existir um remote e ele apontar para um repositório antigo, não fazer push automaticamente. Informar e pedir confirmação antes de qualquer publicação.

### 2. Commit local

Se houver mudanças, criar um commit local com mensagem clara. Se não houver mudanças, informar que está tudo sincronizado.

### 3. Push seguro

Antes de qualquer push:

1. Verificar `git remote -v`.
2. Confirmar que o remote não aponta para o repositório original antigo.
3. Se não existir um remote novo do Athos, fazer apenas commit local e informar que a publicação precisa ser configurada manualmente.
4. Nunca inventar URL de repositório.

### 4. Erros

Se o push falhar:

- explicar o erro de forma simples
- não tentar reescrever histórico sem confirmação
- sugerir que o usuário configure um remote novo ou corrija o existente

## Regras

- Nunca usar `--force` sem confirmação.
- Nunca rodar `git reset --hard` sem confirmação explícita.
- Nunca fazer push para um remote antigo sem autorização.
- Se o remote ainda apontar para a fonte original, bloquear o push e informar claramente.
- Se não houver remote novo, manter apenas o commit local.
