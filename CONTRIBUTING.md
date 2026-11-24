# Como a Kio trabalha

Regras curtas para três pessoas não se atropelarem. Vale para todos os repos da AI-kio.

## Onde fica cada coisa

| Repo | O quê |
|---|---|
| `zapbot` | Bot de WhatsApp com RAG e agendamento |
| `kio-landing` | Landing page |
| `kio-ops` | Tudo que não é código: comercial, piloto, propostas, contratos |

Tudo aparece num quadro só: **Project "Kio"** na organização.

## As 6 regras

1. **Sem issue, não tem trabalho.** Até "ligar para a clínica X" vira issue (no `kio-ops`).
2. **Uma pessoa responsável por issue.** Dois responsáveis = nenhum.
3. **No máximo 2 itens em "Fazendo" por pessoa.** Termine antes de começar outra.
4. **Branch com o número da issue:** `42-confirmacao-agendamento`. O PR leva `Closes #42`.
5. **Merge na `main` só com CI verde e revisão de outra pessoa.** Quem abriu não aprova o próprio PR.
6. **A conversa sobre a tarefa fica na issue**, não no WhatsApp. Decisão tomada em call vira comentário.

## Fluxo do quadro

`Backlog` → `Pronto` → `Fazendo` → `Revisão` → `Feito`

- **Backlog:** ideia registrada, ainda não priorizada.
- **Pronto:** tem objetivo, critério de pronto e tamanho P ou M. Pode pegar.
- **Fazendo:** tem responsável e alguém está mexendo agora.
- **Revisão:** PR aberto (move sozinho).
- **Feito:** PR mergeado ou issue fechada (move sozinho).

Item tamanho **G** não entra em "Pronto": quebre em partes menores.

## Campos

- **Prioridade:** P0 = urgente/cliente parado · P1 = próximo · P2 = algum dia
- **Tamanho:** P até meio dia · M até 2 dias · G quebrar
- **Área:** Produto · Comercial · Infra

## Labels

`bug` · `feature` · `chore` · `comercial` · `bloqueado` (diga no comentário o que está bloqueando e quem destrava).

## Milestones

Milestone é **entrega com data**, nunca categoria. No máximo 2–3 abertos. Mesmo nome em todos os repos envolvidos.

## Ritual

**Segunda-feira, 30 min, olhando o quadro:**
1. O que fecha esta semana?
2. Quem pega o quê?
3. O que está bloqueado e quem destrava?

O resto é assíncrono, nos comentários das issues.
