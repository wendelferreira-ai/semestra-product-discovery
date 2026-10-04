# Do Semestra ao Vende Fácil: Case de Product Discovery e Validação

> Dois ciclos de hipótese → experimento → evidência → decisão em **uma semana**. O primeiro produto não gerou nenhum interesse e foi pivotado; o segundo foi testado com pessoas reais medindo **ação**, não opinião.

**Autor:** [SEU NOME] · **Disciplina:** Metodologias Ágeis e Validação de Produtos · **Período:** 30/09 a 07/10/2026
**🎥 Vídeo pitch:** [LINK]

---

## Resumo em 30 segundos

| | Ciclo 1: Semestra | Ciclo 2: Vende Fácil |
|---|---|---|
| **Ideia** | IA transforma planos de ensino no cronograma do semestre | Manda a foto de algo parado em casa e recebe o preço e o anúncio prontos |
| **Público** | Universitários | Família, amigos e colegas com itens parados |
| **Experimento** | Landing page + formulário, divulgados em grupo da turma | Concierge (Mágico de Oz) por WhatsApp individual |
| **Resultado** | **0 inscrições em 29 pessoas, em 4 dias** | [PREENCHER] |
| **Decisão** | **Pivotar** | [PREENCHER] |

---

## Ciclo 1: Semestra (30/09 a 04/10)

**Problema:** universitários recebem prazos espalhados (PDF, AVA, WhatsApp) e são pegos de surpresa.
**Hipótese de valor:** ≥ 20% dos visitantes da landing page se inscreveriam para testar.

**Experimento:** landing page com formulário "Quero testar", divulgada no grupo de WhatsApp da turma (30 membros) → [hipóteses](ciclo-1-semestra/01-parte-teorica.md) · [landing](ciclo-1-semestra/03-experimento/landing-page/index.html) · [registro](ciclo-1-semestra/04-evidencias/registro-divulgacao.md)

**Resultado:** nenhuma inscrição, nenhuma pergunta e nenhuma reação no grupo em 4 dias ([evidências](ciclo-1-semestra/04-evidencias/)).

**Decisão: PIVOTAR** → [resultado e justificativa](ciclo-1-semestra/05-resultado-e-decisao.md)

**O que aprendemos e levamos para o Ciclo 2:**
1. Post em grupo não é recrutamento → **convite individual**.
2. Esforço inicial alto (buscar PDFs) mata a adesão → **pedir só uma foto**.
3. Opinião é fraca, especialmente de pessoas próximas → **medir uma ação** (publicar o anúncio).

---

## Ciclo 2: Vende Fácil (04/10 a 06/10)

### Problema
Quase toda casa tem objetos parados que o dono gostaria de vender, mas não vende por causa do **trabalho de começar**: descobrir o preço, escrever o anúncio, fotografar e negociar.

### Hipóteses
| # | Hipótese | Meta |
|---|---|---|
| H1 · Problema | Pessoas têm itens parados e não vendem por causa do preço/anúncio/trabalho | ≥ 60% |
| H2 · Solução | Preço + anúncio gerados por IA a partir de uma foto são úteis e confiáveis | Utilidade ≥ 4/5 e ≥ 60% acham o preço justo |
| **H3 · Valor** | **Com o anúncio pronto, as pessoas de fato anunciam** | **≥ 40% publicam até 06/10** |

Detalhes, MVP e regra de decisão: [01-parte-teorica.md](ciclo-2-vende-facil/01-parte-teorica.md) · Canvas: [02-canvas](ciclo-2-vende-facil/02-canvas/canvas.md)

### Experimento: concierge MVP
Nenhuma linha de código. O autor faz o papel do produto:
1. Pergunta sobre o problema, sem falar da solução → [mensagens](ciclo-2-vende-facil/03-experimento/mensagens-whatsapp.md)
2. Recebe a foto, gera preço e anúncio com IA ([prompt](ciclo-2-vende-facil/03-experimento/prompt-concierge.md)) e **confere o preço em 3 anúncios reais**
3. Entrega o anúncio pronto e, no dia seguinte, pergunta: **publicou?**
4. Formulário de 1 minuto → [perguntas](ciclo-2-vende-facil/03-experimento/formulario-avaliacao.md)

### Evidências
[PREENCHER: n participantes, perfil e datas. Inserir 2 ou 3 prints (conversa + anúncio publicado, sem telefones).] → [04-evidencias/](ciclo-2-vende-facil/04-evidencias/)

### Resultados
| Hipótese | Meta | Resultado | Status |
|---|---|---|---|
| H1 | ≥ 60% | [ ] | [ ] |
| H2 · utilidade | ≥ 4/5 | [ ] | [ ] |
| H2 · preço justo | ≥ 60% | [ ] | [ ] |
| **H3 · publicou** | **≥ 40%** | [ ] | [ ] |

**Principais padrões:** [3 bullets com citação, ver [sintese.md](ciclo-2-vende-facil/05-analise/sintese.md)]

### Decisão final
**[PERSEVERAR / AJUSTAR / PIVOTAR / ABANDONAR]**: [justificativa ligada à regra pré-definida]

**Próximo passo recomendado:** [ ]

---

## Aprendizados do processo
- **Confirmado:** [ ]
- **Contrariado:** [ ]
- **Sobre o método:** testar barato e rápido permitiu descartar a primeira ideia em 4 dias, sem escrever código.

## Uso de IA
A IA apoiou a geração de ideias (inclusive as do pivô), a estruturação de hipóteses, a execução dos concierges e o agrupamento de feedbacks. **Nenhuma conclusão se apoia em respostas de IA**: todas vêm do que pessoas reais disseram e, principalmente, **fizeram**. Registro completo: [diario-ia.md](diario-ia.md).

## Estrutura do repositório
```
README.md                  O case completo
CRONOGRAMA.md              Plano da semana (incluindo o pivô)
diario-ia.md               Como a IA foi usada, e onde a decisão foi humana
06-pitch/                  Roteiro do vídeo
ciclo-1-semestra/          Hipóteses, canvas, landing, evidências e decisão de pivotar
ciclo-2-vende-facil/       Hipóteses, canvas, concierge, evidências e síntese
```
