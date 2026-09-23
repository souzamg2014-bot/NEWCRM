# Bloco 6: testar na prática, com o exemplo TinTAi

## Controle

- Status: roteiro do teste e escopo da identidade visual do produto rascunhados; teste em si e identidade visual ainda não executados.
- Depende de: `bloco-05-construir-com-ia.md` (o CRM precisa estar construído, em pelo menos um dos dois cenários, antes de testar).
- Pergunta do bloco: como o TinTAi usaria o CRM num dia real de trabalho, e o que a interface (telas, paleta de cores, logo) precisa comunicar?

## 1. O que "testar na prática" significa nesse bloco

Simular o uso do TinTAi - CRM ao longo de um dia (ou uma semana) de trabalho, seguindo o fluxo definido no bloco 3, com dados fictícios, nos dois cenários da série (A, sofisticado, e B, local). O objetivo é registrar onde o fluxo funciona e onde trava, não só mostrar a ferramenta pronta funcionando sem atrito.

## 2. Cenário de teste: um dia do TinTAi

Roteiro de teste sugerido, ainda a validar com Marcelo:

1. De manhã, chega uma indicação por WhatsApp. TinTAi registra o contato e envia orçamento pelo link do bloco 5.
2. Um cliente de dias atrás responde aceitando um orçamento parado. TinTAi agenda a execução.
3. TinTAi executa um serviço já agendado e lança a conclusão, com custo real diferente do orçado.
4. No fim do dia, TinTAi lança as despesas do dia no fluxo de caixa e confere se o salário do mês já está reservado (bloco 4, seção 3).
5. Um cliente antigo recebe um lembrete de repintura (recorrência, bloco 3, etapa 5).

Esse roteiro ainda não foi executado; é a base para gravar o teste quando o CRM estiver pronto em algum dos dois cenários.

## 3. O que observar durante o teste

- Em qual etapa do fluxo (bloco 3) falta campo ou sobra campo.
- Se o Cenário A e o Cenário B se comportam de formas diferentes pro mesmo roteiro.
- Se as integrações do bloco 5 (WhatsApp, e-mail, agenda) realmente economizam trabalho ou só adicionam passos.
- Se a separação entre salário e lucro (bloco 4, seção 3) fica clara na tela, ou só no banco de dados.
- Onde uma pessoa sem contexto técnico se confundiria usando o sistema.

Nenhuma observação real existe ainda; esta seção lista o que procurar, não o que foi encontrado.

## 4. Identidade visual do produto TinTAi - CRM

Importante não confundir com a identidade visual fixa do perfil pessoal de Marcelo (usada nos carrosséis, definida em `AGENTS.md`). Aqui é a identidade visual do próprio produto que está sendo construído dentro da série:

- Logo do TinTAi.
- Paleta de cores do produto (pode ou não ter relação com a paleta do perfil pessoal; a decidir).
- Mapeamento de UI/UX: quais telas existem (contatos/orçamentos, agenda, financeiro/caixa, execução), a hierarquia entre elas, e o que aparece primeiro quando o TinTAi abre o sistema de manhã.

Nenhum desses itens foi desenhado ainda. A recomendação é desenhar a interface depois do teste da seção 2 e 3, para que as telas reflitam o que o uso real exige, e não o contrário.

## 5. Pendências

- Definir a própria identidade visual (logo, paleta, telas) do TinTAi - CRM.
- Validar ou ajustar o roteiro de teste da seção 2 com Marcelo.
- Decidir se o teste é feito só num cenário (A ou B) primeiro, ou nos dois em paralelo.
- Formato de publicação (vídeo ou carrossel), ainda em aberto para todos os blocos.

## 6. Próximo passo

Construir o suficiente do bloco 5 pra rodar o roteiro da seção 2, registrar as fricções reais encontradas, e só então desenhar logo, paleta e telas do TinTAi - CRM com base no que o teste mostrou ser necessário.
