# Bloco 4: organizar os dados, com o exemplo TinTAi

## Controle

- Status: primeira modelagem de dados rascunhada a partir do fluxo em `bloco-03-fluxo.md`.
- Depende de: `bloco-03-fluxo.md`.
- Pergunta do bloco: como os itens registrados em cada etapa do fluxo viram uma estrutura de dados organizada?

## 1. Registros que não devem se misturar

O bloco 1 já alertava: pessoa, oportunidade e compra precisam ser diferenciadas na modelagem. Para o TinTAi, isso se traduz em cinco registros distintos:

- **Contato**: a pessoa que pediu orçamento.
- **Orçamento**: uma oportunidade específica, ligada a um contato.
- **Serviço executado**: o que de fato foi feito, ligado a um orçamento aceito.
- **Lançamento financeiro**: cada entrada ou saída do caixa, incluindo o salário retirado.
- **Lembrete**: uma ação futura, ligada a um contato ou serviço.

Um mesmo contato pode ter vários orçamentos ao longo do tempo (novo ambiente, indicação de repintura), então orçamento não deve viver dentro do cadastro do contato, e sim referenciá-lo.

## 2. Campos candidatos por registro

| Registro | Campos candidatos |
|---|---|
| Contato | Nome, telefone, origem (indicação, Instagram, outro), pedidos ou preferências específicas |
| Orçamento | Contato vinculado, descrição do serviço, valor orçado, custo estimado, data de envio, prazo de validade, status (aceito, recusado, em dúvida), motivo se recusado |
| Serviço executado | Orçamento vinculado, data de início, data de conclusão, custo real, valor final recebido |
| Lançamento financeiro | Tipo (entrada ou saída), categoria (material, deslocamento, salário, outra despesa), valor, data, serviço vinculado quando houver |
| Lembrete | Tipo (follow-up de orçamento, recorrência, indicação), data, contato ou serviço vinculado |

São campos candidatos, não uma lista fechada. Alguns podem se juntar ou desaparecer quando o fluxo for testado na prática (bloco 6).

## 3. Onde entra o salário / pró-labore

O salário não é um campo separado do resto: é um lançamento financeiro do tipo saída, na categoria "salário", lançado com regularidade (por exemplo, mensal). O lucro real da empresa só aparece depois de descontar essa saída, e não antes. É essa estrutura de dados que sustenta a clareza mencionada no bloco 2: sem o lançamento de salário separado, o caixa positivo pode esconder que não sobra nada além do que o TinTAi já retiraria de qualquer forma pra viver.

## 4. O que ainda é hipótese de modelagem

- Se "orçamento" e "serviço executado" devem ser o mesmo registro com status diferentes, ou dois registros separados como proposto aqui.
- Se lembretes precisam de um registro próprio ou podem viver como um campo de data dentro de orçamento e serviço.
- Se um único cadastro de contato basta ou se, com o tempo, será preciso separar cliente de indicador.

## 5. Próximo passo

Testar esse desenho com uma situação fictícia completa (do contato ao pós-venda) antes de fechar os campos definitivos. Isso é trabalho do bloco 6 (testar na prática), depois de construir com IA no bloco 5.
