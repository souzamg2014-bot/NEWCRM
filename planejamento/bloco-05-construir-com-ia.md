# Bloco 5: construir com IA, com o exemplo TinTAi

## Controle

- Status: dois cenários de arquitetura definidos (sofisticado e local); integração de WhatsApp definida como link direto, sem robô; as 5 integrações valem para os dois cenários; repositório GitHub confirmado; armazenamento local do Cenário B definido como pasta com arquivos simples. Falta executar as checklists de preparação.
- Depende de: `bloco-04-dados.md` (a modelagem que a IA vai usar como base pra construir, em qualquer um dos dois cenários).
- Pergunta do bloco: como organizar arquitetura, contas e ambiente antes de deixar a IA construir, em dois cenários diferentes, e como ensinar integrações reais sem travar no que é fictício?

## 1. Ferramentas de Marcelo, e por que ensinar também a via mais simples

Fluxo que Marcelo usa na prática, referência do Cenário A (seção 2):

- **GitHub**: versionamento e histórico público da construção (a série já usa o repositório NEWCRM, citado em `briefing.md`).
- **Vercel**: hospedagem e deploy do front-end.
- **Supabase**: banco de dados e autenticação.
- **VS Code**: IDE onde o trabalho acontece.
- **Claude Code**: agente de IA que executa a construção dentro do VS Code.

Ponto de ensino que Marcelo pediu para deixar explícito: quem não usa IDE também consegue começar, usando o chat do Claude ou do ChatGPT direto pra gerar uma primeira versão simples, sem instalar nada.

## 2. Dois cenários de construção

Marcelo quer mostrar, lado a lado, dois caminhos possíveis para o mesmo TinTAi - CRM.

Marcelo confirmou que o projeto será público no repositório já existente: https://github.com/souzamg2014-bot/NEWCRM. O código dos dois cenários é versionado ali, lado a lado.

### Cenário A: versão sofisticada, hospedada

- Repositório NEWCRM no GitHub.
- Banco de dados no Supabase, estruturado a partir dos 5 registros do bloco 4.
- Deploy do front-end na Vercel.
- Claude Code como agente que recebe a documentação dos blocos 1 a 4 como instrução e implementa.

Objetivo didático: mostrar como fica um produto pronto pra escalar e ser usado por qualquer cliente real.

### Cenário B: versão local, sem nuvem

- Tudo roda na própria máquina do TinTAi, sem depender de Vercel ou Supabase para funcionar.
- Dados guardados localmente numa pasta com arquivos simples, sem banco de dados dedicado.
- Um arquivo de execução (script ou atalho) sobe o CRM localmente, sem exigir conhecimento técnico de quem for usar.
- O código também é versionado no repositório NEWCRM, mesmo não sendo necessário pra esse cenário rodar; é só pra manter o projeto público e documentado.

Objetivo didático: mostrar que dá pra ter uma primeira versão útil sem depender de contas, custo de nuvem ou conhecimento avançado. É o caminho de quem quer só começar a organizar o próprio negócio.

Os dois cenários são arquitetura proposta, ainda não implementada. Fato já verificado (bloco 1, briefing): o repositório NEWCRM existe no GitHub e estava vazio na consulta de 22/09/2026. Como os dois cenários vão morar no mesmo repositório, a organização das pastas (uma para cada cenário) fica pra quando a IA começar a construir.

## 3. Preparação antes de a IA executar

### Checklist comum aos dois cenários

- [ ] Repositório NEWCRM organizado (branch principal, README inicial, pastas separadas por cenário)
- [ ] Ambiente local com VS Code e Claude Code configurados

### Checklist extra do Cenário A (sofisticado)

- [ ] Estrutura de pastas do projeto (front-end, back-end/API se houver, documentação)
- [ ] Conta e projeto criados no Supabase
- [ ] Conta e projeto criados na Vercel, conectados ao repositório

### Checklist extra do Cenário B (local)

- [ ] Estrutura de pastas do projeto local, com a pasta de dados simples já criada
- [ ] Criar o arquivo de execução que sobe o CRM localmente

Nenhum item das duas listas está confirmado como concluído. É a checklist que o bloco vai mostrar sendo executada, passo a passo, em cada cenário.

## 4. O momento de partir pra IA

Quando a checklist do cenário escolhido estiver pronta, a IA recebe a arquitetura correspondente e a modelagem dos blocos 2 a 4 como instrução e começa a implementar. O ponto que a série quer deixar visível é o mesmo nos dois cenários: o trabalho de preparação manual que antecede a IA "apertar o play".

## 5. Integrações a ensinar

| Integração | Pra que serve no TinTAi | Como funciona | Implementar de fato? |
|---|---|---|---|
| WhatsApp | Onde a maior parte da demanda do TinTAi chega | Um botão que abre o WhatsApp do cliente já com uma mensagem automática preenchida (link direto, sem robô, sem API paga, sem aprovação de conta comercial) | Sim, é simples; vale para os dois cenários |
| E-mail | Enviar orçamento e confirmações ao cliente | Conectar um serviço de e-mail transacional | A decidir se implementa de fato; vale para os dois cenários |
| Agenda | Marcar visitas e execuções, evitar conflito de horário | Integração com um calendário | A decidir se implementa de fato; vale para os dois cenários |
| Instagram | Outra origem de contato do TinTAi | Integração com a API da Meta pra captar leads | Provavelmente só demonstrar, por causa da aprovação de app na Meta; vale para os dois cenários quando implementada |
| Gateway de pagamento | Receber pagamento de orçamentos aprovados | Conectar um gateway de pagamento | Ambiente de testes/sandbox pode permitir demonstrar sem dinheiro real; vale para os dois cenários |

Decisão já dada por Marcelo: nem toda integração precisa ser implementada de ponta a ponta. Quando alguma exigir aprovação externa, conta comercial verificada ou outro requisito que não se sustenta num projeto fictício, a série explica o conceito, mostra a tela de configuração e a lógica de código, e é transparente sobre o que não foi de fato ativado.

## 6. Pendências

- Decidir, das integrações restantes (e-mail, agenda, Instagram, pagamento), quais realmente vão ser implementadas de ponta a ponta.
- Definir a organização de pastas dentro do repositório NEWCRM para separar os dois cenários, quando a IA começar a construir.
- Formato de publicação (vídeo ou carrossel), ainda em aberto para todos os blocos.

## 7. Próximo passo

Executar as duas checklists da seção 3 e documentar o resultado real (o que foi criado, prints, links) em `registro-da-trilha.md` antes de considerar o bloco 5 fechado.
