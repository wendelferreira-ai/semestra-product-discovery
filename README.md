# Semestra — Case de Product Discovery e Validação

> Vale a pena construir um assistente de IA que transforma planos de ensino no cronograma do semestre? Este case documenta **uma semana** de hipóteses, experimento com usuários reais e a decisão baseada em evidências.

**Autor:** [SEU NOME] · **Disciplina:** Metodologias Ágeis e Validação de Produtos · **Período:** 30/09 – 07/10/2026
**🎥 Vídeo pitch:** [LINK] · **🌐 Landing page:** [wendelferreira-ai.github.io/semestra-product-discovery/03-experimento/landing-page/](https://wendelferreira-ai.github.io/semestra-product-discovery/03-experimento/landing-page/)

---

## 1. Problema
Universitários recebem prazos e avaliações espalhados em várias fontes (plano de ensino em PDF, AVA, e-mail, WhatsApp, avisos em sala). Consolidar tudo é manual e raramente é feito, e o resultado são entregas descobertas em cima da hora e semanas sobrecarregadas.

**Público:** graduandos com 4+ disciplinas, especialmente quem trabalha ou estagia.

## 2. Hipóteses
| # | Hipótese | Meta |
|---|---|---|
| H1 · Problema | Universitários são surpreendidos por prazos porque a informação está dispersa | ≥ 60% relatam surpresa no último semestre e usam ≥ 2 fontes |
| H2 · Solução | Um cronograma gerado por IA a partir do plano de ensino é útil e confiável | Utilidade ≥ 4/5 e ≥ 80% de datas corretas |
| H3 · Valor | Estudantes querem continuar usando | ≥ 50% querem para o próximo semestre; ≥ 20% de conversão na landing |

Detalhes, MVP e regra de decisão: [01-parte-teorica.md](01-parte-teorica.md) · Canvas: [02-canvas/canvas.md](02-canvas/canvas.md)

## 3. Experimento
**Concierge MVP + landing page (fake door).** Sem código de produto:
1. Entrevista de problema (sem mencionar a solução) → [roteiro](03-experimento/roteiro-entrevista.md)
2. O aluno envia o plano de ensino; eu gero o cronograma com IA ([prompt](03-experimento/prompt-concierge.md)), confiro as datas e devolvo tabela + arquivo `.ics`
3. Formulário pós-uso após 2–3 dias → [perguntas](03-experimento/formulario-pos-teste.md)
4. Em paralelo: [landing page](03-experimento/landing-page/index.html) divulgada em grupos de turma

## 4. Evidências
[PREENCHER — resumo: n participantes, cursos, datas. Link para [04-evidencias/](04-evidencias/). Inclua 2–3 prints anonimizados aqui.]

## 5. Resultados
| Hipótese | Meta | Resultado | Status |
|---|---|---|---|
| H1 | ≥ 60% | [ ] | [ ] |
| H2 · utilidade | ≥ 4/5 | [ ] | [ ] |
| H2 · acurácia | ≥ 80% | [ ] | [ ] |
| H3 · continuidade | ≥ 50% | [ ] | [ ] |
| H3 · landing | ≥ 20% | [ ] | [ ] |

**Principais padrões:** [3 bullets com citação — ver [05-analise/sintese.md](05-analise/sintese.md)]

## 6. Aprendizados
- **Confirmado:** [ ]
- **Contrariado:** [ ]
- **Surpresa:** [ ]

## 7. Decisão final
**[PERSEVERAR / AJUSTAR / PIVOTAR / ABANDONAR]** — [justificativa ligando dados à regra pré-definida]

**Próximo passo recomendado:** [ ]

## 8. Uso de IA
A IA apoiou exploração de ideias, estruturação de hipóteses, execução do concierge e agrupamento de feedbacks. **Nenhuma conclusão se apoia em respostas de IA**: todas vêm de dados de usuários reais. Registro completo: [diario-ia.md](diario-ia.md).

## Estrutura do repositório
```
01-parte-teorica.md      Hipóteses, MVP, critérios e regra de decisão
02-canvas/               Lean Canvas + Value Proposition Canvas (v1 e v2)
03-experimento/          Roteiro, prompt do concierge, formulários, landing page
04-evidencias/           Dados brutos anonimizados e prints
05-analise/              Síntese, comparação e decisão
06-pitch/                Roteiro do vídeo
diario-ia.md             Como a IA foi usada
CRONOGRAMA.md            Plano da semana
```
