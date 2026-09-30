# Evidências

Tudo que comprova que o experimento aconteceu com pessoas reais. Anonimize sempre (P01, P02…).

> 🔒 **Repositório público.** Guarde prints sem borrar, planos de ensino recebidos e arquivos `.ics` dos participantes em `04-evidencias/brutos/` — essa pasta é ignorada pelo Git e nunca é publicada. Só entra aqui o que já estiver anonimizado.

| Arquivo / pasta | Conteúdo |
|---|---|
| `registro-testes.csv` | Uma linha por participante, preenchida logo após a entrevista + concierge |
| `respostas-formulario.csv` | Export do Google Forms pós-teste |
| `landing-cliques.png` | Print do contador de cliques do link encurtado |
| `landing-respostas.csv` | Export do formulário "Quero testar" |
| `prints/` | Conversas de WhatsApp (nome e foto borrados), cronogramas entregues, calendário importado |
| `consentimentos.md` | Lista P01…P08 com data e "consentiu verbalmente em ___" |

### Como preencher as colunas-chave do CSV
- `n_fontes_prazos`: quantas fontes diferentes a pessoa citou na pergunta 2 → usado na **H1**
- `teve_surpresa_prazo_ultimo_semestre`: sim/não (pergunta 3–4) → **H1**
- `maior_dor_pergunta8`: resposta resumida → detecta **pivô**
- `datas_extraidas` / `datas_corretas`: sua conferência do resultado da IA → **H2 (acurácia)**
- `reacao_oferta`: "aceitou na hora", "pediu p/ mais disciplinas", "hesitou", "recusou" → sinal de **H3**
