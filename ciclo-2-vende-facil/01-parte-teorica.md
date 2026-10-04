# Ciclo 2 · Parte Teórica: Hipóteses e Estratégia de Validação

**Produto (nome provisório):** Vende Fácil: manda a foto de algo que quer vender e recebe o preço sugerido e o anúncio pronto
**Autor:** [SEU NOME] · **Disciplina:** Metodologias Ágeis e Validação de Produtos · **Data:** 04/10/2026

> Origem: pivô decidido ao fim do [Ciclo 1 (Semestra)](../ciclo-1-semestra/05-resultado-e-decisao.md). Este documento é escrito e **congelado antes** do experimento.

---

## 1. Problema, público e oportunidade

**Problema.** Quase toda casa tem objetos parados (bicicleta, eletrônico antigo, roupa, móvel, brinquedo) que o dono até gostaria de vender, mas não vende. O motivo raramente é falta de comprador: é o **trabalho de começar**. É preciso descobrir quanto pedir, escrever um anúncio que convença, tirar fotos boas e responder curiosos. Sem saber o preço, a pessoa tem medo de vender barato demais ou de anunciar caro e ninguém chamar, e adia indefinidamente.

**Público inicial.** Adultos de 25 a 60 anos, acessíveis por contato direto (família, amigos, colegas de trabalho), que usam WhatsApp diariamente e têm pelo menos um item parado em casa.

**Oportunidade.** Modelos de IA multimodais identificam um objeto por foto e escrevem textos de venda em segundos. Combinado a uma checagem rápida de preços reais em anúncios parecidos, isso reduz o "trabalho de começar" de 30-60 minutos para uma foto.

## 2. Hipóteses

| # | Tipo | Hipótese | Métrica e meta |
|---|---|---|---|
| H1 | **Problema** | Acreditamos que as pessoas têm itens parados que gostariam de vender, mas não vendem por causa do trabalho de precificar e anunciar. | ≥ **60%** dos convidados têm ≥ 1 item parado há 3+ meses que gostariam de vender **e** citam preço, anúncio ou "dá trabalho" como motivo de ainda não ter vendido. |
| H2 | **Solução** | Acreditamos que preço sugerido + anúncio pronto, gerados por IA a partir de uma foto, são úteis e confiáveis. | Nota média de utilidade ≥ **4/5** **e** ≥ **60%** consideram o preço sugerido "justo". |
| H3 | **Valor** *(principal)* | Acreditamos que, com o anúncio pronto, as pessoas de fato anunciam. | ≥ **40%** dos testadores **publicam o anúncio** até 06/10 às 12h, com print ou link como evidência. |
| H3b | Valor (secundária) | Acreditamos que querem usar de novo. | ≥ **30%** mandam um 2º item sem que o autor peça. |
| H3c | Valor (informativa) | Acreditamos que parte pagaria pelo serviço. | % que pagaria por anúncio ou por comissão na venda. *(não decide sozinha)* |

**Metas em números, com 5 participantes:** H1 = pelo menos **3 de 5** · H2 preço justo = pelo menos **3 de 5** · H3 publicou = pelo menos **2 de 5** · H3b 2º item = pelo menos **2 de 5**. Os percentuais de H2 e H3 contam só quem recebeu o anúncio.

**Hipótese mais arriscada:** H3. Pessoas próximas tendem a elogiar qualquer coisa (viés de simpatia), então **opinião vale pouco aqui**. A prova de valor é a **ação**: publicar o anúncio.

## 3. Solução proposta e definição do MVP

**Visão de produto (não será construída agora).** Um contato de WhatsApp ou app: a pessoa manda fotos, a IA identifica o item, pesquisa preços de anúncios parecidos, sugere preço de anúncio e preço mínimo, escreve título e descrição, e publica direto na OLX ou no Marketplace.

**MVP = Concierge / Mágico de Oz, por WhatsApp individual:**
1. A pessoa manda foto(s) do item e responde 5 perguntas rápidas.
2. O autor roda um prompt estruturado em um assistente de IA → [prompt-concierge.md](03-experimento/prompt-concierge.md).
3. O autor **confere o preço** em 3 anúncios parecidos (OLX/Marketplace) e ajusta.
4. Devolve: faixa de preço, título, descrição, dicas de foto e respostas prontas para compradores.
5. No dia seguinte, pergunta se publicou e pede o print.

**Fora do escopo:** app, publicação automática, pesquisa automática de preços, intermediação da venda.

**Por que esse MVP?** Testa a hipótese mais arriscada (as pessoas agem?) com custo de horas. Aplicando o aprendizado do Ciclo 1: **convite individual** e **esforço mínimo** (uma foto).

## 4. Uso de IA no processo de discovery

| Etapa | Como a IA foi usada | O que foi decisão humana |
|---|---|---|
| Pivô | Gerar alternativas de produto testáveis com amigos e família | Escolha do Vende Fácil (ação observável + esforço mínimo) |
| Hipóteses | Sugerir formato testável e métricas | Metas numéricas e foco na métrica comportamental |
| MVP | Identificar o item pela foto, sugerir preço, escrever o anúncio | **Conferência do preço** em anúncios reais antes de cada entrega |
| Síntese | Agrupar feedbacks por tema | Interpretação, padrões e decisão |

Registro detalhado: [diario-ia.md](../diario-ia.md). **A IA não valida mercado:** as conclusões vêm do que as pessoas **fizeram**.

## 5. Experimento e critérios de sucesso

| Item | Definição |
|---|---|
| Formato | Perguntas de problema (texto ou áudio) → concierge → acompanhamento "publicou?" → formulário curto |
| Amostra | 5 pessoas entre família, amigos e colegas (V01 a V05), com 1 ou 2 reservas caso alguém não responda |
| Período | 04/10 a 06/10/2026 (12h) |
| Dados quantitativos | % com item parado; motivos; nota de utilidade; % preço justo; **% que publicou**; % que mandou 2º item; diferença entre o preço da IA e o preço de mercado |
| Dados qualitativos | Frases literais, objeções, motivos para não publicar |
| Evidências | Prints das conversas e dos anúncios publicados (sem telefones), CSV do formulário |

## 6. Critério de decisão (definido antes do experimento)

| Resultado | Decisão |
|---|---|
| H1, H2 e H3 atingem a meta | **Perseverar**: próximo passo é automatizar a pesquisa de preço |
| H1 atingida; H2 **ou** H3 abaixo da meta, com feedback claro do que corrigir (ex.: preço desconfiável, texto genérico) | **Ajustar** a solução e repetir |
| H1 atingida, mas a barreira principal é outra (ex.: medo de golpe, logística de entrega, falta de tempo para negociar) | **Pivotar** a solução para essa barreira |
| H1 < 40% | **Abandonar** a hipótese |
| H1 entre 40% e 60% | **Ajustar** o público antes de qualquer solução |
