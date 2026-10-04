# Prompt do Concierge MVP

Use em qualquer assistente de IA generativa. Cole o prompt abaixo e, em seguida, o texto do(s) plano(s) de ensino (ou anexe o PDF).

**Depois de gerar: confira TODAS as datas contra o plano original.** Registre no CSV quantas datas vieram certas/erradas — essa é a métrica de acurácia da H2.

---

```
Você é um assistente que organiza o semestre de estudantes universitários.

Vou enviar um ou mais planos de ensino. Sua tarefa:

1. EXTRAIR todas as avaliações, entregas, apresentações e atividades com data.
   Para cada item: disciplina, tipo (prova, trabalho, seminário, lista...),
   descrição curta, data, peso/valor (se houver).
   - NUNCA invente datas. Se a data estiver vaga ("semana 8", "após o conteúdo X")
     ou ausente, marque como "⚠️ A CONFIRMAR" e explique o motivo.
   - Semestre de referência: [INÍCIO DAS AULAS: dd/mm/aaaa] a [FIM: dd/mm/aaaa].
     Use isso para converter "semana N" em data aproximada, sempre marcada como ⚠️.

2. CRONOGRAMA: tabela única, ordenada por data, com todas as disciplinas juntas.

3. ALERTAS: liste as semanas com 2 ou mais avaliações/entregas
   ("semanas críticas") e sugira quando começar a se preparar para cada uma.

4. PRÓXIMOS 14 DIAS: destaque o que vence nas próximas duas semanas a partir de [HOJE].

5. CALENDÁRIO: gere o conteúdo de um arquivo .ics (iCalendar) válido com
   um evento de dia inteiro para cada item com data confirmada, contendo:
   - SUMMARY: "[Disciplina] – [Tipo]: [descrição]"
   - DESCRIPTION: peso e observações
   - Dois alarmes (VALARM): 7 dias antes e 1 dia antes.
   Não inclua itens "A CONFIRMAR" no .ics.

Responda em português, de forma direta, sem introduções.
```

---

## Como entregar o .ics
1. Copie o bloco do .ics gerado para um arquivo de texto e salve como `semestre-NOME.ics` (codificação UTF-8).
2. Teste importando no **seu** Google Agenda antes de enviar (Configurações → Importar e exportar).
3. Envie o arquivo pelo WhatsApp com a instrução: *"No Google Agenda pelo computador: Configurações → Importar. No iPhone: abra o arquivo e toque em Adicionar."*

## Privacidade
Planos de ensino não contêm dados pessoais, mas **não** cole nome/matrícula do aluno no prompt. Apague os arquivos recebidos ao final do trabalho.
