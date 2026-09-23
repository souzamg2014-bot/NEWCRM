# Plano de produção da série TinTAi - CRM

## Controle

- Status: plano validado por Marcelo em 22/09/2026. É o guia de execução da série a partir daqui.
- Como usar este arquivo: seguir a ordem das fases; marcar `[x]` ao concluir cada item. Se uma fase mudar de escopo ou ordem durante a execução, registrar a mudança em `registro-da-trilha.md` antes de só editar este arquivo, pra manter o histórico coerente.
- Regra que continua valendo: o e-book (Fase 8) só é consolidado no final, com a experiência real já registrada.

## Fase 1: fechar e publicar o bloco 1 (o problema)

- [ ] Revisar e aprovar o texto de Tela 1 / Tela 2 / Tela 3 e a legenda (rascunho já feito nesta conversa, com base em `bloco-01-pensar.md`)
- [ ] Decidir formato: vídeo, carrossel, ou os dois
- [ ] Se vídeo: gravar a partir das tomadas sugeridas em `bloco-01-pensar.md`, seção 7
- [ ] Se carrossel: preencher `carrossel/conteudo.json` e exportar pelo template
- [ ] Revisar legenda e hashtags
- [ ] Mover a proposta fechada para `conteudos/em-revisao/`, depois para `aprovados/` quando Marcelo confirmar
- [ ] Publicar (estreia pretendida: 26/09/2026)
- [ ] Criar o destaque do Instagram para a série (nome a definir) e fixar o primeiro conteúdo nele

## Fase 2: construir o Cenário B do bloco 5 (local, sem nuvem)

Checklist técnica detalhada, a partir de `bloco-05-construir-com-ia.md` e `bloco-04-dados.md`:

- [ ] Criar uma pasta para o Cenário B dentro do repositório NEWCRM
- [ ] Criar a pasta de dados simples, um arquivo por registro: contatos, orçamentos, serviços executados, lançamentos financeiros, lembretes (`bloco-04-dados.md`, seção 2)
- [ ] Criar o arquivo de execução que sobe o CRM localmente (mesmo padrão já usado neste projeto em `carrossel/iniciar.cmd` e `publicador/iniciar.cmd`: um script que inicia um servidor local e abre no navegador)
- [ ] Implementar as 5 telas do fluxo comercial: contato, orçamento, decisão do cliente, execução, pós-venda (`bloco-03-fluxo.md`)
- [ ] Implementar o botão de WhatsApp: link direto com mensagem preenchida, sem robô (`bloco-05-construir-com-ia.md`, seção 5)
- [ ] Implementar o lançamento financeiro e a separação salário/lucro (`bloco-04-dados.md`, seção 3)
- [ ] Deixar a IA (Claude Code) executar essa construção a partir da documentação dos blocos 1 a 4
- [ ] Versionar e publicar no repositório NEWCRM

## Fase 3: gravar e publicar os blocos 2, 3 e 4

Pode rodar em paralelo à Fase 2, já que não depende da construção.

- [ ] Bloco 2 (`bloco-02-primeira-versao.md`): roteirizar, gravar ou diagramar, publicar
- [ ] Bloco 3 (`bloco-03-fluxo.md`): roteirizar, gravar ou diagramar, publicar
- [ ] Bloco 4 (`bloco-04-dados.md`): roteirizar, gravar ou diagramar, publicar
- [ ] Atualizar o destaque do Instagram a cada publicação
- [ ] Atualizar `conteudos/painel.md` a cada publicação

## Fase 4: testar o Cenário B na prática (bloco 6) e desenhar a identidade visual

- [ ] Rodar o roteiro de teste de `bloco-06-testar-na-pratica.md`, seção 2, no Cenário B já construído
- [ ] Registrar cada fricção encontrada em `registro-da-trilha.md`
- [ ] Gravar o teste mostrando a tela do sistema em uso, não só falando sobre ele
- [ ] A partir do que o teste mostrou, desenhar logo, paleta de cores e telas do TinTAi - CRM (`bloco-06-testar-na-pratica.md`, seção 4)
- [ ] Publicar o bloco 6 (vídeo do teste, com ou sem revelar a identidade visual junto)

## Fase 5: construir o Cenário A (sofisticado)

- [ ] Criar conta e projeto no Supabase
- [ ] Modelar as tabelas a partir de `bloco-04-dados.md`, seção 2 (contato, orçamento, serviço executado, lançamento financeiro, lembrete)
- [ ] Criar conta e projeto na Vercel, conectados ao repositório NEWCRM
- [ ] Aplicar a identidade visual desenhada na Fase 4
- [ ] Reaproveitar a lógica já validada no Cenário B (fluxo, integrações, separação salário/lucro)
- [ ] Deploy e publicação do link

## Fase 6: rodar o ciclo de uso e estresse (bloco 7) nos dois cenários

- [ ] Definir se o uso será real ou simulado (`bloco-07-colocar-em-uso.md`, seção 3)
- [ ] Rodar o ciclo: usar, coletar erros, ajustar, testar de novo (`bloco-07-colocar-em-uso.md`, seção 1)
- [ ] Estressar o sistema nos dois cenários (`bloco-07-colocar-em-uso.md`, seção 2)
- [ ] Registrar cada erro relevante em `registro-da-trilha.md`
- [ ] Gravar e publicar o bloco 7 com os erros reais encontrados (a transparência sobre os erros é parte do conteúdo)

## Fase 7: fechar o bloco 8 (consertos e roadmap)

- [ ] Separar, da lista de erros da Fase 6, o que é conserto imediato e o que é ideia de roadmap (`bloco-08-evoluir-com-evidencias.md`, seção 2)
- [ ] Consertar o que for prioridade
- [ ] Preencher o roadmap (`bloco-08-evoluir-com-evidencias.md`, seção 3) só com itens que vieram de evidência real
- [ ] Publicar o bloco 8

## Fase 8: consolidar o e-book completo, formato curso

- [ ] Reunir os 8 blocos (`bloco-01` a `bloco-08`) e os registros de `registro-da-trilha.md`
- [ ] Escrever cada capítulo com: contexto, decisão e motivo, o que foi implementado com evidência, aprendizado ou erro encontrado, e uma pergunta ou exercício curto pro leitor aplicar no próprio negócio
- [ ] Revisar fatos, números e afirmações contra os registros reais, não contra a memória de como a série "deveria" ter acontecido
- [ ] Diagramar (o projeto já tem um e-book publicado em `ebook/` que pode servir de referência de formato)
- [ ] Publicar o e-book e anunciar nos posts e destaques

## Checklist mestre

| Fase | O que entrega | Status |
|---|---|---|
| 1 | Bloco 1 publicado + destaque criado | A iniciar |
| 2 | Cenário B funcionando | A iniciar |
| 3 | Blocos 2, 3 e 4 publicados | A iniciar |
| 4 | Bloco 6 testado + identidade visual desenhada | A iniciar |
| 5 | Cenário A funcionando | A iniciar |
| 6 | Bloco 7 com erros reais registrados | A iniciar |
| 7 | Bloco 8 fechado (consertos + roadmap) | A iniciar |
| 8 | E-book publicado | A iniciar |

## Observação

Este plano é um guia, não um roteiro rígido. As fases 2 e 3 podem rodar em paralelo; as demais dependem da fase anterior ter gerado evidência real antes de avançar.
