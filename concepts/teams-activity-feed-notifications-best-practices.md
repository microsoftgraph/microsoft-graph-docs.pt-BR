---
title: Práticas recomendadas para o uso Microsoft Teams de feed de atividade
description: Este artigo fornece práticas recomendadas e exemplos para trabalhar com notificações de feed de atividade no Microsoft Graph.
author: KirtiPereira
ms.localizationpriority: medium
ms.prod: teamwork
ms.openlocfilehash: 8ebb19f3b10a85862be2d12eeb61a96d33ed40bc
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335805"
---
# <a name="best-practices-for-using-microsoft-teams-activity-feed-notifications"></a>Práticas recomendadas para o uso Microsoft Teams de feed de atividade

Este artigo aborda as práticas recomendadas para o uso Microsoft Teams notificações de feed de atividade no Microsoft Graph. Essas práticas recomendadas se aplicam a:
* Criando notificações de chamada para ação
* Solicitando respostas a notificações
* Criando notificações sobre eventos externos

A imagem a seguir mostra um exemplo de uma notificação de feed de atividade no Teams:

![Captura de tela de um aplicativo Teams exibição de notificação de feed de atividade.](./images/activity-feed-notification.png)

Ao implementar notificações de feed de atividade, lembre-se dos seguintes pontos:
* As notificações de notificação do notificação redirecionam os usuários para o feed de atividades, não para o aplicativo. Para ver outra atividade, os usuários devem selecionar a notificação associada no feed de atividades.
* Os usuários podem gerenciar as configurações de notificação somente depois que o aplicativo selecionado envia uma notificação.
* O ícone de cada notificação está incluído no manifesto do aplicativo. O Microsoft Graph não dá suporte à personalização do ícone.
* As notificações de prioridade não são suportadas.

## <a name="enhance-the-notification-experience"></a>Aprimorar a experiência de notificação

Microsoft Teams exibe notificações em formatos de feed de atividade e notificação de notificação. Os usuários recebem notificações de várias fontes em chats, canais, reuniões ou outros aplicativos. Para aprimorar a experiência do usuário, aplique as seguintes recomendações:

* Localize o conteúdo em um notificação ou feed. A localização só acontece se o conteúdo do aplicativo estiver [localizado](/microsoftteams/platform/concepts/build-and-test/apps-localization).
* Forneça títulos e descrições apropriados para seus **Tipos de Atividade**. Use títulos curtos **, como @mention** **e Comunicados**. Evite títulos longos, como **Atividade de usuário mencionada e** **atividade de criação post.**
* As notificações devem transmitir informações importantes que são relevantes para o usuário. Por exemplo, *Diego atribuiu um tíquete de vendas a você* é uma mensagem relevante; *Joni deixou a equipe de vendas* não.
* Evite o envio de notificações promocionais de natureza, como *Experimentar o novo recurso no aplicativo Cycling*.
* Evite notificações duplicadas de mensagens bot e notificações de feed de atividade. Para obter mais informações, consulte [activity feed notifications or bot framework messages](#activity-feed-notifications-or-bot-framework-messages).
* Use a **seção visualização de** texto em notificações. Forneça informações para ajudar o usuário a determinar a importância da notificação e tomar medidas, se necessário.
* Não adicione um ponto no final do título de notificação, para ser consistente com todas as outras configurações de notificação no Teams.
* Tornar clara a relação entre a notificação e seu conteúdo para o usuário. Por exemplo, quando um usuário recebe uma notificação para aprovar uma licença, a notificação deve redirecioná-la para a seção correspondente do aplicativo. Se a notificação pertence à remoção ou exclusão de entidades, como usuários e tarefas, direcionar o destinatário para o conteúdo e indicar a ação necessária.
* Certifique-se de que a experiência de feed seja autoconstruidora. Por exemplo, quaisquer pop-ups e modais devem permanecer no aplicativo.
* Verifique se seu aplicativo não envia mais de 10 notificações por minuto, por usuário. As notificações serão automaticamente aceleradas se a contagem exceder 10.
* Verifique se o tempo de carregamento do aplicativo não afeta negativamente a experiência dos usuários quando alternam entre notificações no feed.
* Informe o usuário sobre o período de armazenamento de notificações no feed de atividades. Em Microsoft Teams, o período de armazenamento é de 30 dias.
    > [!NOTE]
    > O limite de armazenamento de 30 dias se aplica a todas as notificações. Não é específico para notificações enviadas por meio da API de notificações de feed de atividade.

## <a name="activity-feed-notifications-or-bot-framework-messages"></a>Notificações de feed de atividade ou mensagens de estrutura de bot

Você pode usar notificações de feed de atividade ou mensagens de estrutura de bot, mas não use ambos os tipos de notificação. As seções a seguir descrevem os tipos de notificação e quando usar cada um. 

### <a name="activity-feed-notifications"></a>Notificações de feed de atividades

As notificações de feed de atividade aparecem no feed Teams atividade e podem incluir links para vários locais. Essas notificações: 
* Permitir que o usuário tome medidas ou triagem da notificação.
* Leve o usuário a uma guia em um chat ou canal, um aplicativo pessoal ou uma mensagem de chat ou canal. 

A API de notificações de feed de atividade permite que os usuários configurem notificações **para cada tipo** de notificação a partir das configurações de notificação.

Se você usar notificações de feed de atividade, esteja ciente de que seu aplicativo pode enviar notificações duplas, se ele enviar notificações de bot para chats ou canais e também para o feed de atividades. Envie notificações duplas somente se o cenário exigir. 

Use notificações delegadas para criar uma experiência de notificação melhor. A API de notificação de feed de atividade pode enviar chamadas delegadas ou somente de aplicativos. Em chamadas delegadas, o remetente da notificação aparece como o usuário que iniciou a notificação e, em chamadas somente de aplicativo, o remetente aparece como o aplicativo. 

Você pode atualizar uma notificação de feed de atividade existente em vez de criar uma nova notificação usando o *parâmetro chainId* .

### <a name="bot-framework-messages"></a>Mensagens de estrutura bot

As mensagens bot são entregues como mensagens de chat ou canal. Se o usuário ativar notificações de chat ou canal, as notificações disparadas serão enviadas como mensagens de chat ou canal. Para enviar mensagens de bot, *@mention* o nome do usuário para que a notificação apareça no feed de atividades.

É útil que o alerta seja consumido como uma mensagem de chat ou canal; por exemplo, uma mensagem que é consumida por todos os membros do canal.

## <a name="see-also"></a>Confira também

[Criar notificações de feed de atividade para Microsoft Teams](/microsoftteams/platform/concepts/design/activity-feed-notifications?tabs=mobile) 