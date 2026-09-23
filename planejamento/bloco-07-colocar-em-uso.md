# Bloco 7: colocar em uso, com o exemplo TinTAi

## Controle

- Status: lógica do bloco definida por Marcelo; execução depende do CRM já testado no bloco 6.
- Depende de: `bloco-06-testar-na-pratica.md` (o roteiro de teste e as fricções já observadas).
- Pergunta do bloco: o que acontece quando o TinTAi - CRM sai do teste controlado e vai pro uso do dia a dia, e como usar isso pra encontrar problemas que o teste não mostrou?

## 1. O ciclo do bloco

Definido por Marcelo: colocar em uso, coletar erros, ajustar, testar de novo, e estressar o sistema. É um ciclo que se repete, não um passo único:

1. Usar o CRM numa rotina real (ou simulada com volume real de dados fictícios).
2. Coletar os erros e travas que aparecerem nesse uso.
3. Ajustar o que for possível corrigir de imediato.
4. Testar de novo pra confirmar que o ajuste funcionou.
5. Estressar o sistema: forçar situações fora do comum, pra ver onde ele quebra antes do cliente real quebrar.

## 2. O que significa "estressar o sistema" no caso do TinTAi

- Muitos orçamentos e contatos ao mesmo tempo, simulando um pico de demanda.
- Dados incompletos ou fora do padrão esperado (cliente sem telefone, orçamento sem prazo de validade).
- Uso fora do fluxo pensado no bloco 3 (por exemplo, marcar execução sem orçamento aceito).
- A mesma carga aplicada nos dois cenários (A e B), pra ver se algum dos dois quebra primeiro.

## 3. Uso real ou simulado

Ainda a decidir com Marcelo: se o "colocar em uso" é literal, com algum profissional de verdade testando (o que exigiria cuidado extra com dados reais de terceiros), ou se continua simulado, com Marcelo mesmo gerando um volume alto de dados fictícios do TinTAi. Enquanto não for decidido, tratar como simulado.

## 4. Como registrar os erros encontrados

Cada erro relevante entra como um registro em `registro-da-trilha.md`, seguindo o modelo padrão (pergunta, decisão, evidência), pra que o bloco 8 tenha uma lista real de problemas pra consertar, e não uma lista reconstruída de memória.

## 5. Pendências

- Decidir se o uso é real ou simulado.
- Definir o volume e o tipo de estresse a aplicar em cada cenário.
- Formato de publicação (vídeo ou carrossel), ainda em aberto para todos os blocos.

## 6. Próximo passo

Rodar o ciclo da seção 1 até esgotar os ajustes simples, registrar cada erro encontrado, e então passar pro bloco 8 para separar o que já foi consertado do que vira roadmap.
