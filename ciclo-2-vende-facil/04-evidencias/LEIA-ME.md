# Evidências: Ciclo 2 (Vende Fácil)

Tudo que comprova que o experimento aconteceu com pessoas reais.

| Arquivo / pasta | Conteúdo |
|---|---|
| [registro-convites.md](registro-convites.md) | Quando e por qual canal cada pessoa foi convidada, a mensagem enviada e os desvios do protocolo |
| [registro-testes.csv](registro-testes.csv) | Uma linha por convidado (V01, V02…): respostas de problema, preço da IA × mercado, publicou ou não |
| `prints/form-curto-respostas-*.png` | Resumo das respostas do formulário curto, como aparece no Google Forms |
| `entregas/` | Um arquivo por participante: checagem de preço em anúncios reais e anúncio entregue |
| `prints/` | Telas reais das conversas, das entregas e dos **anúncios publicados** |
| `brutos/` | Originais e fotos recebidas, **ignorado pelo Git e nunca publicado** |

## Regras de privacidade (repositório público)
- **Prints com a tela real e inteira**, incluindo nomes de grupos e pessoas, para comprovar que o teste aconteceu. Nos documentos de análise, cada pessoa aparece pelo código (V01 a V05).
- **Telefones, e-mails, CPF e comprovantes de Pix de terceiros sempre cobertos.**
- **Mensagens pessoais anteriores ao teste ficam borradas**: aparecem na tela, mas não dá para ler.
- Nos prints de anúncios publicados, cubra também telefone e endereço exato, se aparecerem.
- Fotos de itens podem aparecer, com **reflexos da pessoa e do ambiente borrados**. A foto original fica só em `brutos/`.

## Colunas-chave do CSV
| Coluna | Hipótese |
|---|---|
| `tem_item_parado`, `motivo_nao_vendeu` | **H1** (o motivo é preço/anúncio/trabalho?) |
| `preco_ia_anuncio`, `preco_mercado_medio`, `diferenca_pct` | **H2** (a IA acerta o preço?) |
| `publicou`, `evidencia_publicacao` | **H3** (a pessoa agiu?) |
| `mandou_2o_item` | **H3b** (quer de novo, sem pedir?) |
