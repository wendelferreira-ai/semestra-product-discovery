# Prompt do Concierge — Vende Fácil

Use em qualquer assistente de IA que aceite imagens. Cole o prompt, anexe as fotos e preencha as respostas da pessoa.

**Depois de gerar, SEMPRE confira o preço** (passo obrigatório, mais abaixo). Essa conferência é a métrica de confiabilidade da H2.

---

```
Você ajuda pessoas comuns a vender objetos usados na OLX e no Facebook Marketplace, no Brasil.

Vou enviar fotos de um item e as informações que o dono passou.
Dono informou:
- O que é: [ ]
- Marca/modelo (se souber): [ ]
- Tempo de uso: [ ]
- Estado e defeitos: [ ]
- Acompanha (caixa, carregador, acessórios): [ ]
- Cidade/bairro: [ ]
- Prefere vender rápido ou pelo melhor preço: [ ]

Responda nesta ordem, em português, direto ao ponto:

1. IDENTIFICAÇÃO: o que você vê nas fotos. Se algo não estiver claro
   (modelo, defeito, tamanho), diga o que falta. NUNCA invente
   especificações que não aparecem nas fotos nem foram informadas.

2. PREÇO:
   - Preço de anúncio (com margem para negociar)
   - Preço mínimo (abaixo disso não vale a pena)
   - Em 1 frase: de onde vem a estimativa e o grau de incerteza.
   Considere o perfil "vender rápido" ou "melhor preço".

3. TÍTULO: até 60 caracteres, com marca/modelo e o principal atrativo.

4. DESCRIÇÃO: pronta para colar, até 600 caracteres, com estado real
   (incluindo defeitos), o que acompanha, motivo da venda (genérico),
   retirada/entrega e forma de pagamento. Tom simpático e honesto.

5. CATEGORIA sugerida na OLX e no Marketplace.

6. FOTOS: 3 dicas práticas para melhorar as fotos DESTE item.

7. RESPOSTAS PRONTAS:
   - "Ainda está disponível?"
   - "Faz por [valor abaixo do mínimo]?"
   - "Aceita troca?"

8. SEGURANÇA: 3 cuidados para não cair em golpe nesta venda.
```

---

## ✅ Conferência de preço (obrigatória, ~3 minutos)
1. Pesquise o item na **OLX** e no **Marketplace** (mesma marca, modelo e estado, de preferência na mesma região).
2. Anote o preço de **3 anúncios parecidos**.
3. Calcule a média e compare com o preço de anúncio da IA.
4. Se a diferença passar de 20%, ajuste o preço antes de entregar e anote o motivo.
5. Registre no [registro-testes.csv](../04-evidencias/registro-testes.csv): `preco_ia_anuncio`, `preco_mercado_medio`, `diferenca_pct`, `preco_entregue`.

> Essa etapa é o "humano no circuito" do MVP. No produto real, ela seria automatizada; aqui ela mede **o quanto a IA sozinha acerta**.

## Privacidade
- Não coloque nome, telefone ou endereço completo da pessoa no prompt (use só o bairro).
- Fotos recebidas ficam em `04-evidencias/brutos/` (fora do Git).
