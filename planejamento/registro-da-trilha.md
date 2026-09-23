# Registro contínuo da trilha de CRM

## Regra de trabalho

Registrar durante a construção. Consolidar o e-book somente no final, por orientação de Marcelo. Documentar ideias como ideias, funcionalidades como implementadas apenas quando verificadas e resultados apenas quando observados.

## Mapa dos blocos

| Bloco | Tema | Estado |
|---|---|---|
| 1 | Pensar o problema e o papel do CRM | Relato recebido e organizado; exemplo TinTAi definido |
| 2 | Definir a primeira versão | Escopo definido (`bloco-02-primeira-versao.md`) |
| 3 | Desenhar o fluxo | Fluxo comercial rascunhado (`bloco-03-fluxo.md`) |
| 4 | Organizar os dados | Modelagem inicial rascunhada (`bloco-04-dados.md`) |
| 5 | Construir com IA | Dois cenários definidos, repositório NEWCRM confirmado para ambos, integrações e armazenamento local decididos (`bloco-05-construir-com-ia.md`); execução ainda não iniciada |
| 6 | Testar na prática | Roteiro de teste e escopo de identidade visual rascunhados (`bloco-06-testar-na-pratica.md`); execução ainda não iniciada |
| 7 | Colocar em uso | Ciclo de uso, coleta de erros e estresse do sistema definido (`bloco-07-colocar-em-uso.md`); execução ainda não iniciada |
| 8 | Evoluir com evidências | Regra de separar conserto de roadmap definida (`bloco-08-evoluir-com-evidencias.md`); depende dos erros do bloco 7 |

O mapa organiza o ensino. Na prática, testes podem levar a revisões de fluxo, escopo e dados; registrar esses retornos.

## Registro 001: visão inicial

- Data: 22/09/2026.
- Bloco: 1, pensar.
- Material original: `../../entrada/crm-bloco-01-relato-marcelo.md`.
- Material organizado: `bloco-01-pensar.md`.
- Ideia autoral: relacionar o acompanhamento comercial com o aprendizado de gestão sobre o cliente e o negócio.
- Decisão confirmada: documentar agora para produzir o e-book ao final.
- Hipóteses: utilidade dos dados para aquisição, percepção de valor, recorrência e atuação da equipe.
- Implementação e testes: não realizados neste registro.
- Gravações recebidas: nenhuma vinculada até este registro.
- Publicações: nenhuma desta série vinculada até este registro.
- Próxima decisão: escolher o exemplo de negócio e a tarefa central da primeira versão.

## Registro 002: negócio-exemplo da série

- Data: 22/09/2026.
- Bloco: 2, definir a primeira versão (exemplo entra a partir daqui).
- Pergunta ou problema: qual negócio fictício conduz a série, já levantada como pendência no Registro 001.
- Relato original ou arquivo de origem: conversa direta com Marcelo nesta sessão.
- Alternativas consideradas: nenhuma outra apresentada; Marcelo trouxe a escolha já fechada.
- Decisão e motivo: negócio fictício TinTAi, um pintor profissional autônomo, com alta demanda, que atende sozinho e precisa se organizar tanto para atender bem quanto para enxergar a empresa como negócio e avaliar se dá para escalar e crescer. O produto da série se chama TinTAi - CRM. Motivo: é um perfil brasileiro reconhecível (prestador de serviço individual sobrecarregado), concreto o bastante para exemplos de tela sem expor dados reais de cliente nenhum.
- Hipótese ainda não testada: que esse perfil (autônomo, alta demanda, sem estrutura) generaliza bem para o público amplo da série.
- O que foi implementado, se aplicável: nada; é decisão editorial, sem código ou sistema associado.
- Evidência: este registro.
- Resultado observado: não se aplica ainda.
- O que mudou em relação à decisão anterior: fecha a pendência "qual negócio ou profissional será o exemplo recorrente da série", listada como aberta no Registro 001.
- Próximo passo: usar TinTAi / TinTAi - CRM a partir do roteiro do Episódio 2 (a primeira versão); Episódio 1 (o problema) não depende do exemplo e permanece genérico.
- Possível aprendizado para o e-book: registrar se um exemplo fictício único ao longo de oito blocos ajuda ou limita a variedade de situações ensináveis.

## Registro 003: fluxo do Episódio 2 (TinTAi)

- Data: 22/09/2026.
- Bloco: 2, definir a primeira versão.
- Pergunta ou problema: o que precisa acontecer entre registrar uma conversa e executar o próximo passo, usando TinTAi como exemplo.
- Relato original ou arquivo de origem: conversa direta com Marcelo nesta sessão; desenvolvimento em `bloco-02-fluxo.md`.
- Alternativas consideradas: nenhuma alternativa de fluxo apresentada ainda; primeira proposta de rascunho.
- Decisão e motivo: fluxo em 5 etapas (contato, orçamento, decisão do cliente, execução, pós-venda), cada uma com o que registrar e a próxima ação disparada. Motivo: dar uma resposta concreta e ensinável à pergunta do episódio sem ainda comprometer a modelagem final de dados.
- Hipótese ainda não testada: que o maior risco do TinTAi é perder o fio de conversas já iniciadas, não falta de demanda. Não validada com Marcelo nem com pintor real.
- O que foi implementado, se aplicável: nada; é roteiro editorial.
- Evidência: `bloco-02-fluxo.md`.
- Resultado observado: não se aplica.
- O que mudou em relação à decisão anterior: fecha o Episódio 2 com o exemplo TinTAi definido no Registro 002.
- Próximo passo: Marcelo decide formato (vídeo ou carrossel) e confirma ou ajusta a hipótese da seção 1 de `bloco-02-fluxo.md`; depois adaptar para o formato escolhido.
- Possível aprendizado para o e-book: registrar se a hipótese "perder o fio da conversa" se confirma como o problema real de negócios de alta demanda e baixa estrutura.

## Registro 004: escopo ampliado do TinTAi - CRM

- Data: 22/09/2026.
- Bloco: 2, definir a primeira versão.
- Pergunta ou problema: o fluxo comercial (Registro 003) bastava para a primeira versão do TinTAi - CRM?
- Relato original ou arquivo de origem: conversa direta com Marcelo nesta sessão.
- Alternativas consideradas: manter a primeira versão só no fluxo comercial (contato a pós-venda), deixando custo, caixa e salário para blocos futuros.
- Decisão e motivo: Marcelo optou por já incluir controle de custos, prazos, agenda, recorrência, lembretes, contatos, pedidos específicos do cliente, orçamentos, fluxo de caixa e um "salário" (pró-labore) pensado pela categoria. Motivo dado por ele: esse tipo de profissional recebe demanda por indicação, tem alta demanda mas pouco tempo pra pensar no negócio como um todo; separar salário de lucro traz clareza pra decidir investir e escalar.
- Hipótese ainda não testada: que não separar salário de lucro é o que impede esse perfil de enxergar se o negócio comporta crescer. Leitura de Marcelo sobre o perfil, não dado observado.
- O que foi implementado, se aplicável: nada; é decisão de escopo editorial, sem código ou sistema associado.
- Evidência: `bloco-02-fluxo.md`, seção 3.
- Resultado observado: não se aplica.
- O que mudou em relação à decisão anterior: a exclusão de "indicadores de gestão" registrada no Registro 003 (seção "o que fica de fora") foi revertida para fluxo de caixa e salário; CAC continua fora, mas agora por não fazer sentido no perfil (demanda por indicação), não por estar reservado para blocos futuros.
- Próximo passo: Marcelo decide formato (vídeo ou carrossel); se carrossel, provavelmente a série precisa de mais de uma publicação pra cobrir fluxo comercial e escopo financeiro sem sobrecarregar 3 telas.
- Possível aprendizado para o e-book: registrar se dava pra prever, já no bloco 1, que "primeira versão" para esse perfil de profissional exigiria gestão financeira desde o início, não como evolução posterior.

## Registro 005: redistribuição do conteúdo entre os blocos 2, 3 e 4

- Data: 22/09/2026.
- Bloco: reorganização que afeta os blocos 2, 3 e 4.
- Pergunta ou problema: o conteúdo dos Registros 003 e 004 estava todo em `bloco-02-fluxo.md`, misturando definição de escopo (bloco 2), desenho de fluxo (bloco 3) e modelagem de dados (bloco 4).
- Relato original ou arquivo de origem: pedido direto de Marcelo nesta sessão para separar o que já foi falado nos três blocos corretos.
- Alternativas consideradas: manter tudo em um arquivo só por episódio, em vez de seguir o mapa de 8 blocos.
- Decisão e motivo: dividir em `bloco-02-primeira-versao.md` (o que entra e o que fica de fora da primeira versão), `bloco-03-fluxo.md` (a tabela de etapas do fluxo comercial) e `bloco-04-dados.md` (registros e campos candidatos, incluindo onde entra o lançamento de salário/pró-labore). Motivo: manter a trilha coerente com o mapa de 8 blocos para consolidação futura do e-book.
- Hipótese ainda não testada: as hipóteses seguem as mesmas dos Registros 003 e 004 (perder o fio da conversa; não separar salário de lucro impede ver se dá pra crescer), agora distribuídas entre os blocos 2 e 3.
- O que foi implementado, se aplicável: nada; reorganização de documentação.
- Evidência: `bloco-02-primeira-versao.md`, `bloco-03-fluxo.md`, `bloco-04-dados.md`. O arquivo `bloco-02-fluxo.md` foi removido após a redistribuição.
- Resultado observado: não se aplica.
- O que mudou em relação à decisão anterior: os Registros 003 e 004 citavam `bloco-02-fluxo.md` como evidência; esse arquivo não existe mais, o conteúdo está nos três arquivos citados acima.
- Próximo passo: seguir para o bloco 5 (construir com IA) quando Marcelo decidir o formato de publicação dos blocos 2 a 4.
- Possível aprendizado para o e-book: ao trabalhar por episódio de publicação em vez de por bloco do mapa, o conteúdo tende a se misturar; vale já produzir separado por bloco desde o início.

## Registro 006: arquitetura e integrações do bloco 5

- Data: 22/09/2026.
- Bloco: 5, construir com IA.
- Pergunta ou problema: com quais ferramentas e em qual ordem organizar a construção do TinTAi - CRM, e como lidar com integrações que podem esbarrar em requisitos externos num projeto fictício.
- Relato original ou arquivo de origem: conversa direta com Marcelo nesta sessão.
- Alternativas consideradas: nenhuma alternativa de ferramentas apresentada; Marcelo trouxe o próprio fluxo de trabalho já definido.
- Decisão e motivo: usar GitHub, Vercel, Supabase, VS Code e Claude Code (o fluxo real de Marcelo), mas também ensinar a via por chat (Claude ou ChatGPT) pra quem não usa IDE. Preparar pastas e contas antes de deixar a IA executar. Listar 5 integrações (e-mail, agenda, WhatsApp, Instagram, gateway de pagamento) para ensinar o quê e o porquê de cada uma; Marcelo definiu que algumas podem ficar só na demonstração conceitual quando esbarrarem em requisito externo (ex: aprovação de conta comercial) que não se sustenta num projeto fictício.
- Hipótese ainda não testada: nenhuma nova; a arquitetura ainda não foi implementada.
- O que foi implementado, se aplicável: nada; checklist de preparação (seção 3 de `bloco-05-construir-com-ia.md`) ainda não executada.
- Evidência: `bloco-05-construir-com-ia.md`.
- Resultado observado: não se aplica.
- O que mudou em relação à decisão anterior: nenhuma decisão anterior sobre ferramentas existia; este é o primeiro registro do bloco 5.
- Próximo passo: Marcelo decide, integração por integração, o que implementar de fato; depois executar a checklist de preparação (contas, pastas, ambiente).
- Possível aprendizado para o e-book: registrar quais integrações realmente saíram do papel e quais ficaram só como demonstração, e por quê, como exemplo real de escopo em projeto de portfólio.

## Registro 007: WhatsApp simplificado e dois cenários de arquitetura

- Data: 22/09/2026.
- Bloco: 5, construir com IA.
- Pergunta ou problema: a integração de WhatsApp precisa de robô/API, e existe só um caminho de arquitetura pra construir o TinTAi - CRM?
- Relato original ou arquivo de origem: conversa direta com Marcelo nesta sessão.
- Alternativas consideradas: WhatsApp via robô/API (descartado); arquitetura única em nuvem (descartada em favor de dois cenários).
- Decisão e motivo: WhatsApp entra como um botão com link direto e mensagem automática preenchida, sem robô, sem API paga e sem aprovação de conta comercial; é simples e funciona igual nos dois cenários. Além disso, a série mostra dois cenários de construção lado a lado: Cenário A (GitHub, Vercel, Supabase, Claude Code, versão sofisticada e hospedada) e Cenário B (tudo local, sem essas contas, subindo por um arquivo de execução). Motivo: ensinar tanto o caminho "produto pronto pra escalar" quanto o caminho "começar simples, sem depender de nuvem".
- Hipótese ainda não testada: nenhuma nova.
- O que foi implementado, se aplicável: nada; decisão de escopo e arquitetura.
- Evidência: `bloco-05-construir-com-ia.md`, seções 2, 3 e 5 (linha do WhatsApp).
- Resultado observado: não se aplica.
- O que mudou em relação à decisão anterior: o Registro 006 tratava WhatsApp como integração que "provavelmente só demonstrar" por causa de aprovação de API; essa leitura mudou porque a versão que Marcelo quer (link direto) não depende de aprovação nenhuma. O Registro 006 também descrevia só uma arquitetura; agora são duas, em paralelo.
- Próximo passo: definir o formato de armazenamento local do Cenário B e quais das demais integrações (e-mail, agenda, Instagram, pagamento) valem para os dois cenários ou só para o Cenário A.
- Possível aprendizado para o e-book: registrar se mostrar dois cenários lado a lado (sofisticado vs. local) ajuda o público a escolher o caminho certo pro próprio nível, em vez de um único caminho "ideal".

## Registro 008: repositório confirmado, integrações valem para os dois cenários, armazenamento local simples

- Data: 22/09/2026.
- Bloco: 5, construir com IA.
- Pergunta ou problema: as integrações do bloco 5 valem só para um cenário? Qual repositório usar? Qual formato de armazenamento local no Cenário B?
- Relato original ou arquivo de origem: conversa direta com Marcelo nesta sessão; link do repositório enviado por ele: https://github.com/souzamg2014-bot/NEWCRM.
- Alternativas consideradas: banco de dados dedicado para o Cenário B (descartado); repositório novo e separado para cada cenário (descartado).
- Decisão e motivo: as 5 integrações (WhatsApp, e-mail, agenda, Instagram, pagamento) valem para os dois cenários, não só para o sofisticado. O armazenamento local do Cenário B fica numa pasta com arquivos simples, sem banco de dados dedicado ("nada demais", nas palavras de Marcelo). O projeto inteiro, os dois cenários, é publicado no repositório público já existente, NEWCRM.
- Hipótese ainda não testada: nenhuma nova.
- O que foi implementado, se aplicável: nada; decisão de escopo.
- Evidência: `bloco-05-construir-com-ia.md`, seções 2, 3, 5 e 6.
- Resultado observado: não se aplica.
- O que mudou em relação à decisão anterior: os Registros 006 e 007 deixavam em aberto se as integrações valiam para os dois cenários e qual seria o formato de armazenamento do Cenário B; ambos ficam resolvidos aqui. Também fica confirmado que o Cenário B, mesmo rodando sem depender de GitHub, tem seu código publicado ali junto por decisão de manter o projeto público.
- Próximo passo: decidir quais integrações além do WhatsApp serão implementadas de ponta a ponta, e organizar as pastas do repositório para os dois cenários quando a construção começar.
- Possível aprendizado para o e-book: registrar se compartilhar as mesmas integrações entre um cenário simples e um sofisticado facilita ou complica o código, na prática.

## Registro 009: roteiro de teste e identidade visual do produto (bloco 6)

- Data: 22/09/2026.
- Bloco: 6, testar na prática.
- Pergunta ou problema: como mostrar o TinTAi - CRM funcionando num dia real, e quando entra o desenho de UI/UX, paleta e logo do produto.
- Relato original ou arquivo de origem: conversa direta com Marcelo nesta sessão.
- Alternativas considaradas: desenhar a interface antes do teste (descartada; recomendação editorial é testar primeiro, desenhar depois).
- Decisão e motivo: o bloco 6 junta duas coisas pedidas por Marcelo: testar o CRM aplicando situações do dia a dia (roteiro de 5 passos na seção 2 de `bloco-06-testar-na-pratica.md`) e mostrar o mapeamento de UI/UX, paleta de cores e logo do próprio produto TinTAi - CRM, deixando claro que essa identidade é do produto, não do perfil pessoal de Marcelo.
- Hipótese ainda não testada: que desenhar a interface depois do teste, e não antes, evita telas que não correspondem ao uso real. Ainda não validada porque o teste não ocorreu.
- O que foi implementado, se aplicável: nada; nem o teste nem a identidade visual foram executados.
- Evidência: `bloco-06-testar-na-pratica.md`.
- Resultado observado: não se aplica.
- O que mudou em relação à decisão anterior: nenhuma decisão anterior existia sobre o bloco 6; primeiro registro dele.
- Próximo passo: construir o suficiente do bloco 5 pra rodar o roteiro de teste, depois desenhar logo, paleta e telas do produto.
- Possível aprendizado para o e-book: registrar se testar antes de desenhar a interface realmente evitou retrabalho, como argumento prático pro método ensinado na série.

## Registro 010: lógica dos blocos 7 e 8

- Data: 22/09/2026.
- Bloco: 7 (colocar em uso) e 8 (evoluir com evidências).
- Pergunta ou problema: qual é o ciclo de trabalho desses dois blocos finais da trilha.
- Relato original ou arquivo de origem: conversa direta com Marcelo nesta sessão.
- Alternativas consideradas: nenhuma; Marcelo definiu a lógica diretamente.
- Decisão e motivo: bloco 7 é um ciclo de usar, coletar erros, ajustar, testar de novo e estressar o sistema (detalhado em `bloco-07-colocar-em-uso.md`). Bloco 8 é consertar o que o bloco 7 encontrar e registrar o que não for consertado agora como roadmap de evolução (detalhado em `bloco-08-evoluir-com-evidencias.md`). Motivo: fechar a trilha com evidência real de uso, não com uma lista de melhorias imaginadas sem teste.
- Hipótese ainda não testada: nenhuma nova; ambos os blocos dependem de dados que ainda não existem (nem o bloco 5 foi construído, nem o bloco 6 testado).
- O que foi implementado, se aplicável: nada; é a lógica editorial dos dois blocos finais.
- Evidência: `bloco-07-colocar-em-uso.md`, `bloco-08-evoluir-com-evidencias.md`.
- Resultado observado: não se aplica.
- O que mudou em relação à decisão anterior: nenhuma decisão anterior existia sobre os blocos 7 e 8; primeiro registro de ambos.
- Próximo passo: construir (bloco 5) e testar (bloco 6) antes de ter conteúdo real para rodar o ciclo do bloco 7 e preencher o roadmap do bloco 8.
- Possível aprendizado para o e-book: usar a lista real de erros do bloco 7 e o roadmap do bloco 8 como o capítulo mais concreto do e-book, por vir de evidência e não de plano.

## Registro 011: plano de produção multi-formato

- Data: 22/09/2026.
- Bloco: transversal, afeta a publicação de todos os 8 blocos.
- Pergunta ou problema: Marcelo quer gravar a construção, gerar um e-book completo em formato de curso, criar posts de apoio, usar destaques do Instagram e produzir reels a partir do mesmo material. Faltava uma ordem de execução.
- Relato original ou arquivo de origem: conversa direta com Marcelo nesta sessão.
- Alternativas consideradas: nenhuma alternativa de ordem apresentada por Marcelo; este é um plano proposto por mim, ainda sem validação dele.
- Decisão e motivo: proposta de plano em `plano-de-producao.md`, priorizando publicar o bloco 1 desde já (não depende de construção) e construir primeiro o Cenário B do bloco 5 (mais rápido, sem contas de nuvem) pra gerar evidência cedo, antes de partir pro Cenário A e pros blocos 6 a 8. O e-book em formato de curso só é consolidado no final, mantendo a regra já registrada no Registro 001.
- Hipótese ainda não testada: que construir o Cenário B primeiro realmente acelera a geração de evidência sem comprometer o Cenário A depois.
- O que foi implementado, se aplicável: nada; é um plano, aguardando validação de Marcelo.
- Evidência: `plano-de-producao.md`.
- Resultado observado: não se aplica.
- O que mudou em relação à decisão anterior: nenhuma ordem de execução existia antes; primeiro registro que propõe uma.
- Próximo passo: Marcelo valida ou ajusta o plano; feito isso, próximo trabalho concreto é fechar o bloco 1 e iniciar a checklist do Cenário B.
- Possível aprendizado para o e-book: registrar se a ordem proposta (publicar cedo, construir o cenário simples primeiro) se confirmou como a mais eficiente pra série.

## Registro 012: plano de produção validado e detalhado

- Data: 22/09/2026.
- Bloco: transversal, guia de execução de todos os 8 blocos.
- Pergunta ou problema: o plano proposto no Registro 011 fazia sentido pra Marcelo, e faltava detalhamento acionável.
- Relato original ou arquivo de origem: conversa direta com Marcelo nesta sessão ("faz sim, cria de forma detalhada pra me ajudar e orientar").
- Alternativas consideradas: nenhuma; Marcelo validou a ordem proposta e pediu detalhamento, não uma ordem alternativa.
- Decisão e motivo: `plano-de-producao.md` reescrito com 8 fases detalhadas (uma checklist acionável por fase) e uma checklist mestre de acompanhamento. Motivo: Marcelo pediu um guia prático pra se orientar durante a execução, não só a ordem em alto nível.
- Hipótese ainda não testada: nenhuma nova; segue a mesma hipótese do Registro 011.
- O que foi implementado, se aplicável: nada da construção em si; é o guia de execução.
- Evidência: `plano-de-producao.md`.
- Resultado observado: não se aplica.
- O que mudou em relação à decisão anterior: o Registro 011 tinha o plano em alto nível, sem checklist; este registro marca a validação de Marcelo e o detalhamento em itens acionáveis.
- Próximo passo: começar pela Fase 1 (fechar e publicar o bloco 1) e, em paralelo, iniciar a Fase 2 (checklist técnica do Cenário B).
- Possível aprendizado para o e-book: registrar se seguir este plano fase a fase, com checklist marcável, ajudou a manter o ritmo da série, como exemplo de organização de projeto pessoal.

## Modelo para os próximos registros

Copiar esta estrutura a cada sessão relevante:

```markdown
## Registro NNN: título

- Data:
- Bloco:
- Pergunta ou problema:
- Relato original ou arquivo de origem:
- Alternativas consideradas:
- Decisão e motivo:
- Hipótese ainda não testada:
- O que foi implementado, se aplicável:
- Evidência: arquivo, commit, captura ou teste:
- Resultado observado:
- O que mudou em relação à decisão anterior:
- Próximo passo:
- Possível aprendizado para o e-book:
```

## Índice das gravações

Ainda sem arquivos recebidos. Marcelo pode continuar depositando os materiais em `conteudos/entrada/` sem organizá-los previamente. Preservar os originais e preencher o índice ao processá-los.

| Arquivo original | Data | Bloco | Trecho inicial/final | Assunto | Uso editorial | Status |
|---|---|---|---|---|---|---|

Registrar a transcrição separadamente do roteiro revisado. Não inventar tempos de vídeo antes de assistir ao arquivo. Vincular cada corte ao original para permitir novas edições e recuperação do contexto no e-book.

## Consolidação final, quando chegar o momento

- Revisar o percurso real dos oito blocos.
- Separar o que foi implementado do que ficou como hipótese ou próximo passo.
- Selecionar exemplos, imagens e trechos com suas fontes.
- Conferir conceitos, métricas e resultados.
- Só então escrever e diagramar o e-book completo.
