---
title: Práticas recomendadas para usar notificações de feed de atividades do Microsoft Teams
description: Obtenha dicas para aprimorar a experiência de notificação do feed de atividades do Microsoft Teams no Microsoft Graph e saiba quando escolher notificações ou mensagens de estrutura de bot.
author: KirtiPereira
ms.localizationpriority: medium
ms.prod: teamwork
ms.openlocfilehash: 37dd5cda8200aeeac0e810ae7a86408f3db876b3
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555868"
---
# <a name="best-practices-for-using-microsoft-teams-activity-feed-notifications"></a>Práticas recomendadas para usar notificações de feed de atividades do Microsoft Teams

Este artigo aborda as práticas recomendadas para usar as notificações do feed de atividades do Microsoft Teams no Microsoft Graph. Essas práticas recomendadas se aplicam a:
* Criando notificações de chamada para ação
* Solicitando respostas a notificações
* Criando notificações sobre eventos externos

A imagem a seguir mostra um exemplo de uma notificação do feed de atividades no Teams:

![Captura de tela de um aplicativo do Teams mostrando a exibição de notificação do feed de atividades.](./images/activity-feed-notification.png)

Ao implementar notificações do feed de atividades, lembre-se dos seguintes pontos:
* As notificações do sistema redirecionam os usuários para o feed de atividades, não para o aplicativo. Para ver outra atividade, os usuários devem selecionar a notificação associada no feed de atividades.
* Os usuários podem gerenciar as configurações de notificação somente depois que o aplicativo selecionado envia uma notificação.
* O ícone de cada notificação está incluído no manifesto do aplicativo. O Microsoft Graph não dá suporte à personalização do ícone.
* Não há suporte para notificações de prioridade.

## <a name="enhance-the-notification-experience"></a>Aprimorar a experiência de notificação

O Microsoft Teams exibe notificações nos formatos de feed de atividades e notificação do sistema. Os usuários recebem notificações de várias fontes em chats, canais, reuniões ou outros aplicativos. Para aprimorar a experiência do usuário, aplique as seguintes recomendações:

* Localize o conteúdo em uma notificação do sistema ou feed. A localização só ocorrerá se o conteúdo do aplicativo [for localizado](/microsoftteams/platform/concepts/build-and-test/apps-localization).
* Forneça títulos e descrições apropriados para seus tipos **de atividade**. Use títulos curtos, como **@mention** **e Comunicados**. Evite títulos longos, como **atividade do usuário mencionada e** atividade **pós-criação**.
* As notificações devem transmitir informações importantes que são relevantes para o usuário. Por exemplo, *Diego atribuiu um tíquete de vendas a você* é uma mensagem relevante; *Joni deixou a equipe de* vendas.
* Evite enviar notificações promocionais por natureza, como *Experimentar o novo recurso no aplicativo de ciclismo*.
* Evite notificações duplicadas de mensagens de bot e notificações do feed de atividades. Para obter mais informações, consulte [escolher notificações do feed de atividades ou mensagens da estrutura do bot](#choose-activity-feed-notifications-or-bot-framework-messages).
* Use a seção **de visualização** de texto em notificações. Forneça informações para ajudar o usuário a determinar a importância da notificação e tomar medidas, se necessário.
* Não adicione um ponto no final do título da notificação para ser consistente com todas as outras configurações de notificação no Teams.
* Torne a relação entre a notificação e seu conteúdo clara para o usuário. Por exemplo, quando um usuário recebe uma notificação para aprovar uma licença, a notificação deve redirecioná-lo para a seção correspondente do aplicativo. Se a notificação pertencer à remoção ou exclusão de entidades, como usuários e tarefas, direcione o destinatário para o conteúdo e indique a ação necessária.
* Verifique se a experiência de feed é autossuficiente. Por exemplo, todos os pop-ups e modais devem permanecer no aplicativo.
* Verifique se seu aplicativo não envia mais de 10 notificações por minuto, por usuário. As notificações serão limitadas automaticamente se a contagem exceder 10.
* Certifique-se de que o tempo de carregamento do aplicativo não afete negativamente a experiência para os usuários quando eles alternam entre notificações no feed.
* Informe o usuário sobre o período de armazenamento de notificações no feed de atividades. No Microsoft Teams, o período de armazenamento é de 30 dias.
    > [!NOTE]
    > O limite de armazenamento de 30 dias se aplica a todas as notificações. Ele não é específico para notificações enviadas por meio da API de notificações do feed de atividades.

## <a name="choose-activity-feed-notifications-or-bot-framework-messages"></a>Escolher notificações do feed de atividades ou mensagens da estrutura do bot

Você pode usar notificações do feed de atividades ou mensagens de estrutura de bot, mas não usar ambos os tipos de notificação. As seções a seguir descrevem os tipos de notificação e quando usar cada um.

### <a name="activity-feed-notifications"></a>Notificações de feed de atividades

As notificações do feed de atividades aparecem no feed de atividades do Teams e podem incluir links para vários locais. Estas notificações: 
* Permitir que o usuário execute uma ação ou faça a triagem da notificação.
* Leve o usuário a uma guia em um chat ou canal, um aplicativo pessoal ou uma mensagem de chat ou canal. 

A API de notificações do feed de atividades permite que os usuários configurem notificações para cada tipo **de notificação** nas configurações de notificação.

Se você usar notificações do feed de atividades, lembre-se de que seu aplicativo pode enviar notificações duplas, se ele enviar notificações de bot para chats ou canais e também para o feed de atividades. Envie notificações duplas somente se o cenário exigir. 

Use notificações delegadas para criar uma melhor experiência de notificação. A API de notificação do feed de atividades pode enviar chamadas delegadas ou somente de aplicativo. Em chamadas delegadas, o remetente da notificação aparece como o usuário que iniciou a notificação e, em chamadas somente de aplicativo, o remetente aparece como o aplicativo. 

Você pode atualizar uma notificação de feed de atividades existente em vez de criar uma nova notificação usando o *parâmetro chainId* .

### <a name="bot-framework-messages"></a>Mensagens do Bot Framework

As mensagens do bot são entregues como mensagens de chat ou canal. Se o usuário ativar notificações de chat ou canal, as notificações disparadas serão enviadas como mensagens de chat ou canal. Para enviar mensagens de bot, *@mention* o nome do usuário para que a notificação apareça no feed de atividades.

É útil que o alerta seja consumido como uma mensagem de chat ou canal; por exemplo, uma mensagem que é consumida por todos os membros do canal.

## <a name="see-also"></a>Confira também

- [Criar notificações do feed de atividades para o Microsoft Teams](/microsoftteams/platform/concepts/design/activity-feed-notifications?tabs=mobile)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)