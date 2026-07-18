---
name: instalar
description: >
  Instala o Athos com uma entrevista guiada, uma pergunta por vez. Preenche a memória operacional, a identidade visual e o contexto inicial sem sobrescrever dados existentes sem confirmação.
---

# /instalar — Instalação inicial do Athos

Essa é a primeira experiência de onboarding do Athos. A instalação deve ser guiada, clara e segura. O objetivo é configurar o contexto inicial do negócio, sem sobrescrever conteúdo real sem autorização.

## Pré-checagem

### 1. Nome da pasta

Identificar o nome atual da pasta. Nomes válidos de referência para o Athos incluem:

- `Athos`
- `athos`
- `athos-main`
- variações equivalentes

Se a pasta ainda tiver um nome genérico ou antigo, não forçar a troca. Apenas registrar o nome atual e indicar que o produto continua sendo Athos.

### 2. Arquivos existentes

Verificar se os seguintes arquivos já existem e possuem conteúdo real:

- `_memoria/empresa.md`
- `_memoria/preferencias.md`
- `_memoria/estrategia.md`
- `identidade/design-guide.md`

Se houver conteúdo preenchido, perguntar:

> "Já existe contexto preenchido aqui. Quer que eu complemente o que falta ou crie um backup antes de atualizar?"

Se não houver conteúdo, seguir direto.

---

## Fase 1 — Perfil operacional

Perguntar uma questão por vez:

1. "Qual perfil melhor descreve sua operação?"
   - Solopreneur
   - Freelancer
   - Agência ou consultoria
   - Empresa

2. "Como você prefere chamar o negócio ou o workspace?"

3. "Qual é o nome do projeto ou do contexto principal que deve ficar visível para o Athos?"

4. "Que tipo de cliente ou público você atende?"

---

## Fase 2 — Contexto do negócio

Perguntar uma por vez:

1. "Em uma frase, o que o seu negócio entrega?"
2. "Quem paga ou quem é o público principal?"
3. "Você opera sozinho ou com equipe? Se houver equipe, descreva a estrutura básica."
4. "Quais são os principais produtos, serviços ou entregas?"

---

## Fase 3 — Tom, preferências e restrições

Perguntar uma por vez:

1. "Me dê um exemplo real de linguagem que você gosta ou que representa bem o seu negócio."
2. "O que você prefere evitar na comunicação?"
3. "Quais são as principais restrições, gargalos ou prioridades atuais?"
4. "Quais ferramentas você usa com frequência?"

---

## Fase 4 — Identidade visual

Perguntar uma por vez:

1. "Você já tem uma identidade visual definida?"
2. "Se sim, envie cores, fontes ou um arquivo de logo. Se não, posso deixar o guia em estado neutro e personalizável."

Se houver material, preencher `identidade/design-guide.md`. Se não houver, manter o arquivo com uma base neutra e profissional.

---

## Fase 5 — Atualização segura de arquivos

Antes de preencher ou substituir qualquer arquivo:

1. Verificar se o arquivo já possui conteúdo real.
2. Criar backup com data e hora quando houver conteúdo preenchido.
3. Se o arquivo existir e estiver preenchido, perguntar se deve:
   - complementar o conteúdo existente
   - criar backup e substituir
   - manter como está

Arquivos alvo:

- `_memoria/empresa.md`
- `_memoria/preferencias.md`
- `_memoria/estrategia.md`
- `identidade/design-guide.md`
- `CLAUDE.md`
- `_memoria/configuracao-athos.md` (criar se ainda não existir)

---

## Fase 6 — Preenchimento dos arquivos

### `_memoria/empresa.md`

Preencher com o contexto operacional capturado nas fases anteriores.

### `_memoria/preferencias.md`

Registrar tom de voz, estilo, restrições e preferências.

### `_memoria/estrategia.md`

Registrar foco atual, gargalos, prioridades e próximos passos.

### `identidade/design-guide.md`

Preencher com base visual, ou deixar a estrutura profissional e neutra quando o usuário ainda não tiver um padrão fechado.

### `_memoria/configuracao-athos.md`

Criar um arquivo com informações principais de configuração do projeto, incluindo:

- nome da empresa
- nome do workspace
- slug do negócio
- perfil operacional
- foco atual
- preferências principais

### `CLAUDE.md`

Atualizar o núcleo do projeto para refletir a configuração inicial do Athos, sem perder a lógica operacional já existente.

---

## Fase 7 — Resumo final

Exibir uma mensagem clara e objetiva no final:

```text
Athos configurado com sucesso.

O sistema já possui o contexto inicial do seu negócio, suas preferências, seu foco atual e as regras principais de operação.

Use /abrir no início de cada sessão para carregar o contexto.
```

---

## Regras

- Nunca sobrescrever conteúdo real sem backup ou confirmação.
- Nunca substituir o nome Athos pelo nome da empresa no produto.
- Manter Athos como nome do produto e separar empresa, workspace e projeto como configurações específicas.
- Fazer uma pergunta por vez.
- Não inventar dados. Quando não houver resposta, registrar de forma neutra e explícita.
- Não fazer promessas de publicação, push ou integração sem confirmação do usuário.

