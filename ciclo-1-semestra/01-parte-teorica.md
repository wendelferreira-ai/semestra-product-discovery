# Ciclo 1 · Parte Teórica: Hipóteses e Estratégia de Validação

> 🔁 **Ciclo encerrado em 04/10/2026 com decisão de PIVOTAR.** Resultado e justificativa: [05-resultado-e-decisao.md](05-resultado-e-decisao.md). Este documento é mantido como estava antes do teste.

**Produto (nome provisório):** Semestra, assistente de IA que transforma planos de ensino em um cronograma do semestre
**Autor:** [SEU NOME] · **Disciplina:** Metodologias Ágeis e Validação de Produtos · **Data:** [DATA]

> ⚠️ Este documento é escrito e **congelado antes** do experimento. Resultados só entram no `README.md` e em `05-analise/sintese.md`.

---

## 1. Problema, público e oportunidade

**Problema.** Universitários recebem as informações de prazos e avaliações espalhadas em várias fontes: plano de ensino em PDF, AVA/Moodle, e-mail, grupos de WhatsApp, avisos em sala. Consolidar tudo exige esforço manual que a maioria não faz, e o resultado é descobrir uma entrega em cima da hora, acumular provas na mesma semana ou perder prazos.

**Público inicial (early adopters).** Estudantes de graduação, cursando 4+ disciplinas simultâneas, que trabalham ou estagiam (menos tempo livre para se organizar).

**Oportunidade.** Os planos de ensino já contêm a maior parte das datas e pesos, mas em texto não estruturado. Modelos de linguagem conseguem extrair essas informações e gerar um calendário acionável em segundos, algo que manualmente leva de 30 min a 1 h por semestre e raramente é feito.

## 2. Hipóteses

| # | Tipo | Hipótese | Métrica e meta |
|---|---|---|---|
| H1 | **Problema** | Acreditamos que universitários com 4+ disciplinas têm dificuldade de acompanhar prazos porque as informações estão dispersas em várias fontes. | ≥ **60%** dos entrevistados relatam ter perdido, quase perdido ou sido surpreendidos por um prazo no último semestre **e** usam ≥ 2 fontes para saber prazos. |
| H2 | **Solução** | Acreditamos que um cronograma gerado por IA a partir do plano de ensino é útil e confiável o suficiente para o aluno usar. | Nota média de utilidade ≥ **4/5** **e** ≥ **80%** das datas extraídas corretas (conferência manual). |
| H3 | **Valor** | Acreditamos que os estudantes querem continuar usando essa solução. | ≥ **50%** dos testadores querem usar para as próximas disciplinas/semestre **e** ≥ **20%** dos visitantes da landing page deixam contato. |
| H3b | Valor (secundária) | Acreditamos que parte dos estudantes pagaria por isso. | ≥ **30%** pagariam ≥ R$ 5/mês. *(informativa, não decide sozinha)* |

**Hipótese mais arriscada:** H1. Se o problema não for frequente e doloroso, nada mais importa. Por isso ela é testada primeiro, antes de qualquer menção à solução.

## 3. Solução proposta e definição do MVP

**Visão de produto (não será construída agora).** O aluno envia os planos de ensino (PDF/foto); a IA extrai avaliações, entregas, datas e pesos; gera um cronograma do semestre, detecta semanas sobrecarregadas, sincroniza com Google Calendar e envia lembretes.

**MVP = Concierge / Mágico de Oz.** Nenhuma linha de código de produto:
1. O aluno envia o plano de ensino por WhatsApp.
2. Eu executo um prompt estruturado em um assistente de IA generativa (`03-experimento/prompt-concierge.md`).
3. Confiro as datas manualmente e devolvo: tabela de entregas, alertas de semanas críticas e um arquivo `.ics` para importar no calendário.

**Complemento: landing page (fake door).** Página explicando a proposta com botão "Quero testar", divulgada em grupos de turma, para medir interesse espontâneo em escala maior do que as entrevistas.

**Por que esse MVP?** Testa o valor entregue (H2 e H3) com custo de horas, não semanas. Se o valor não aparecer com um humano garantindo a qualidade, não aparecerá com um produto automatizado.

**Fora do escopo do MVP:** app, login, integração automática com AVA, notificações push, processamento automático de PDF.

## 4. Uso de IA no processo de discovery

| Etapa | Como a IA foi usada | O que foi decisão humana |
|---|---|---|
| Exploração | Gerar alternativas de problema e público | Escolha do problema (acesso a usuários + frequência da dor) |
| Hipóteses | Sugerir formato testável e métricas | Definição das metas numéricas |
| Roteiro | Revisar perguntas para remover viés/indução | Versão final do roteiro |
| MVP | A própria IA é o "motor" do concierge | Conferência manual de todas as datas antes da entrega |
| Síntese | Agrupar feedbacks por tema | Interpretação, padrões finais e decisão |

Registro detalhado de prompts e decisões: `diario-ia.md`.

**Princípio:** a IA não valida mercado. Nenhuma conclusão deste projeto se apoia em resposta de modelo, apenas em dados de pessoas reais.

## 5. Experimento e critérios de sucesso

| Item | Definição |
|---|---|
| Formato | Entrevista de problema (10 min) → concierge MVP → formulário pós-uso (2-3 dias depois) + landing page em paralelo |
| Amostra | 6-8 universitários (mínimo 5) recrutados em turmas diferentes |
| Duração | 30/09 a 05/10/2026 |
| Dados quantitativos | % com o problema; nº de fontes usadas; nota de utilidade (1-5); % de datas corretas; % que querem continuar; disposição a pagar; conversão da landing |
| Dados qualitativos | Frases literais, alternativas usadas hoje, objeções |
| Critérios de sucesso | Metas da tabela de hipóteses (seção 2) |

## 6. Critério de decisão (definido antes do experimento)

| Resultado | Decisão |
|---|---|
| H1, H2 e H3 atingem a meta | **Perseverar**: próximo passo é automatizar a extração (protótipo funcional) |
| H1 atingida; H2 **ou** H3 abaixo da meta, mas os feedbacks apontam o que corrigir (ex.: formato, confiança nas datas, canal) | **Ajustar** a solução e repetir o ciclo |
| H1 atingida, mas a dor principal relatada é outra (ex.: organizar estudo, não prazos) **ou** o público que mais sente é outro (ex.: calouros, EAD) | **Pivotar** problema ou público |
| H1 < 40% | **Abandonar** a hipótese |
| H1 entre 40% e 60% | Zona cinzenta → **Ajustar** o público-alvo e rodar mais entrevistas antes de qualquer solução |
