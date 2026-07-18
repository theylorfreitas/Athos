---
name: abrir
description: >
  Abre uma sessão de trabalho carregando a memória operacional do Athos e devolve um resumo curto para o usuário. Use quando o usuário disser "abrir", "começar o dia", "/abrir" ou no primeiro turno de uma sessão depois do /instalar.
---

# /abrir — Abertura de sessão

Curto e direto. O objetivo é carregar contexto e devolver uma síntese útil para o usuário começar a trabalhar.

## Workflow

1. Ler, em ordem, os arquivos que existirem:
   - `_memoria/empresa.md`
   - `_memoria/preferencias.md`
   - `_memoria/estrategia.md`
   - `identidade/design-guide.md`

2. Se algum dos arquivos principais estiver ausente ou incompleto, responder de forma objetiva:
   > "Ainda falta contexto inicial em `_memoria/` ou `identidade/`. Quer rodar `/instalar` para completar?"

3. Se tudo estiver disponível, devolver uma mensagem curta no formato:

```text
[Nome do negócio] — [o que faz em 5-8 palavras]
Foco atual: [prioridade da estratégia, em uma frase]
Tom: [resumo de 3-4 palavras do tom de voz]

Pronto. O que vamos fazer?
```

4. Não listar quais arquivos foram lidos. Não confirmar leitura. Só usar o contexto.

## Regras

- Resposta tem que caber em 5 linhas no terminal.
- Não fazer perguntas além de "o que vamos fazer?"
- Se o `design-guide.md` estiver ausente, não mencionar o problema a menos que uma skill visual precise disso.
