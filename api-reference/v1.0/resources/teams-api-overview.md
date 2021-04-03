---
title: Usar o Microsoft Graph API para trabalhar com o Microsoft Teams
description: O Microsoft Teams é um espaço de trabalho baseado em chat no Microsoft 365 que fornece acesso interno a calendários, arquivos, anotações do OneNote, planos do Planner e muito mais.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: 12bfbb201d90a8c35a8d4d1a7a87e91cf9fb28c7
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582589"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Usar o Microsoft Graph API para trabalhar com o Microsoft Teams

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Microsoft Teams é um espaço de trabalho baseado em chat no Microsoft 365 que fornece acesso interno a calendários, arquivos, anotações do OneNote, planos do Planner e muito mais.

## <a name="key-resources-in-microsoft-teams"></a>Principais recursos no Microsoft Teams (visualização)

| Resource | Métodos |
|:---------------|:--------|
|[team](../resources/team.md)| [Listar suas equipes](../api/user-list-joinedteams.md), [listar todas as equipes](/graph/teams-list-all-teams), [criar](../api/team-put-teams.md), [ler](../api/team-get.md), [atualizar](../api/team-update.md), [excluir](../api/group-delete.md), [clonar](../api/team-clone.md), [arquivar](../api/team-archive.md), [cancelar o arquivamento](../api/team-unarchive.md) |
|[group](../resources/group.md)| [Adicionar membro](../api/group-post-members.md),  [remover membro](../api/group-delete-members.md), [adicionar proprietário](../api/group-post-owners.md),  [remover proprietário](../api/group-delete-owners.md), [obter arquivos](drive.md), [obter bloco de anotações](../resources/notebook.md), [obter planos](plannergroup.md), [obter calendário](event.md) |
|[channel](../resources/channel.md)|[Listar](../api/channel-list.md), [criar](../api/channel-post.md), [ler](../api/channel-get.md), [atualizar](../api/channel-patch.md), [excluir](../api/channel-delete.md)|
|[teamsTab](../resources/teamstab.md) |[Listar](../api/channel-list-tabs.md), [criar](../api/channel-post-tabs.md), [ler](../api/channel-get-tabs.md), [atualizar](../api/channel-patch-tabs.md), [excluir](../api/channel-delete-tabs.md) |
|[teamsApp](../resources/teamsapp.md)|[Listar](../api/appcatalogs-list-teamsapps.md), [publicar](../api/teamsapp-publish.md), [atualizar](../api/teamsapp-update.md), [remover](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [Listar](../api/team-list-installedapps.md), [instalar](../api/team-post-installedapps.md), [atualizar](../api/team-delete-installedapps.md), [remover](../api/team-delete-installedapps.md) |
|[chatMessage](../resources/chatmessage.md)| [listar no canal](../api/channel-list-messages.md), [listar no chat](../api/chat-list-messages.md), [enviar](../api/chatmessage-post.md), [ler no canal](../api/chatmessage-get.md), [ler no chat](../api/chatmessage-get.md)|
|[call](../resources/call.md)| [Responder](../api/call-answer.md), [rejeitar](../api/call-reject.md), [redirecionar](../api/call-redirect.md), [ativar mudo](../api/call-mute.md), [desfazer ativar mudo](../api/call-unmute.md), [alterar a função de compartilhamento de tela](../api/call-changescreensharingrole.md), [listar participantes](../api/call-list-participants.md), [convidar participantes](../api/participant-invite.md) |
|[cronograma](../resources/schedule.md)| [Criar ou substituir](../api/team-put-schedule.md), [obter](../api/schedule-get.md), [compartilhar](../api/schedule-share.md) |
|[schedulingGroup](../resources/schedulinggroup.md)| [Criar](../api/schedule-post-schedulinggroups.md), [Listar](../api/schedule-list-schedulinggroups.md), [Obter](../api/schedulinggroup-get.md), [Substituir](../api/schedulinggroup-put.md), [Excluir](../api/schedulinggroup-delete.md) |
|activityFeedNotification| [Enviar notificação ao usuário no escopo de um chat](../api/chat-sendactivitynotification.md), [Enviar notificação ao usuário no escopo de uma equipe](../api/team-sendactivitynotification.md), [Enviar notificação ao usuário no escopo pessoal ](../api/userteamwork-sendactivitynotification.md)|
|[shift](../resources/shift.md)| [Criar](../api/schedule-post-shifts.md), [Listar](../api/schedule-list-shifts.md), [Obter](../api/shift-get.md), [Substituir](../api/shift-put.md), [Excluir](../api/shift-delete.md) |
|[timeOff](../resources/timeoff.md)| [Criar](../api/schedule-post-timesoff.md), [Listar](../api/schedule-list-timesoff.md), [Obter](../api/timeoff-get.md), [Substituir](../api/timeoff-put.md), [Excluir](../api/timeoff-delete.md) |
|[timeOffReason](../resources/timeoffreason.md)| [Criar](../api/schedule-post-timeoffreasons.md), [Listar](../api/schedule-list-timeoffreasons.md), [Obter](../api/timeoffreason-get.md), [Substituir](../api/timeoffreason-put.md), [Excluir](../api/timeoffreason-delete.md) |

## <a name="microsoft-teams-limits"></a>Limites do Microsoft Teams

As limitações de desempenho e de capacidade testadas do Microsoft Teams estão documentadas nas [especificações e limites do Microsoft Teams](/microsoftteams/limits-specifications-teams).
Esses limites aplicam-se diretamente ao usar o Microsoft Teams ou usar as APIs do Microsoft Graph.
Como todas as equipes têm um grupo correspondente, e cada grupo é um objeto de diretório, limites no [número de grupos](/microsoft-365/admin/create-groups/office-365-groups#group-limits) e o [número de objetos de diretório ("recursos")](/azure/active-directory/users-groups-roles/directory-service-limits-restrictions) também podem ser levados em consideração. 

Os arquivos dentro de canais são armazenados no SharePoint. [os limites do SharePoint Online](/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits) se aplicam.

Confira também [redução dos limites dos serviços do Microsoft Teams](/graph/throttling#microsoft-teams-service-limits).

## <a name="teams-and-groups"></a>Equipes e grupos

Na Microsoft Graph, o Microsoft Teams é representado por um recurso de [grupo](../resources/group.md). Os grupos do Microsoft Teams e Microsoft 365 atendem às várias necessidades de colaboração em grupo. Quase todos os recursos baseados em grupo se aplicam aos grupos do Microsoft Teams e do Microsoft 365, como calendário de grupo, arquivos, anotações, fotos, planos e assim por diante. A principal diferença entre uma [equipe](team.md) e um grupo do Microsoft 365 é o modo de comunicação entre os membros. Os membros do Teams se comunicam por meio de chat persistente no contexto de uma equipe específica. Os membros do grupo do Microsoft 365 se comunicam por conversas em grupo, que são conversas de email que ocorrem no contexto de um grupo no Outlook.

Qualquer grupo que tenha uma equipe possui uma propriedade **resourceProvisioningOptions** que contém "Team".

>**Observação:** a propriedade **Group.resourceProvisioningOptions** pode ser alterada.
Não adicione ou remova "Team" dessa coleção; caso contrário, você obterá resultados incorretos ao listar todas as equipes.

Veja a seguir as diferenças no nível da API entre equipes e grupos:

- O chat persistente está disponível apenas para o Microsoft Teams. Esse recurso é representado hierarquicamente pelos recursos [channel](../resources/channel.md) e [chatMessage](../resources/chatmessage.md).
- As conversas em grupo estão disponíveis apenas para grupos do Microsoft 365. Esse recurso é representado hierarquicamente pelos recursos [conversation](../resources/conversation.md), [conversationThread](../resources/conversationthread.md) e [post](../resources/post.md). 
- O método [Listar equipes unidas](../api/user-list-joinedteams.md) se aplica apenas ao Microsoft Teams.
- As [APIs de chamadas e reuniões online](./communications-api-overview.md) aplicam-se apenas ao Microsoft Teams.
- Confira também os [problemas conhecidos](/graph/known-issues) dessas APIs.

>Observação: Se você usar as APIs de grupo em um aplicativo Microsoft Teams, em vez de um aplicativo autônomo, por exemplo, como parte de uma guia ou um bot em execução no Microsoft Teams. Siga as orientações no artigo Uso do Microsoft Graph em suas páginas do Microsoft Teams.

## <a name="membership-changes-in-microsoft-teams"></a>Alterações de associação no Microsoft Teams

Para adicionar membros e proprietários a uma equipe, altere a associação do [grupo](../resources/group.md) com a mesma ID.

| Caso de uso      | Verbo      | URL |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Adicionar membro](../api/group-post-members.md)    | POST      | /groups/{id}/members/$ref  |
| [Remover membro](../api/group-delete-members.md)   | DELETE    | /groups/{id}/members/{userId}/$ref |
| [Adicionar proprietário](../api/group-post-owners.md)     | POST       | /groups/{id}/owners/$ref |
| [Remover proprietário](../api/group-delete-owners.md) | DELETE    | /groups/{id}/owners/{userId}/$ref |
| [Atualizar equipe](../api/team-update.md)  | PATCH     | /teams/{id} |

Recomendamos que, ao adicionar um proprietário, você também adicione esse usuário como membro.
Se uma equipe tiver um proprietário que também não seja um membro, as alterações de propriedade e associação talvez não sejam imediatamente exibidas no Microsoft Teams.
Além disso, aplicativos e APIs diferentes tratam disso de maneira diferente.
Por exemplo, o Microsoft Teams mostrará equipes das quais o usuário é membro ou proprietário, enquanto os cmdlets do PowerShell do Microsoft Teams e a API /me/joinedTeams mostrarão apenas as equipes das quais o usuário é membro.
Para evitar confusão, adicione também todos os proprietários à lista de membros.

Problema conhecido: quando DELETE /groups/{id}/owners é chamado, o usuário também é removido da lista /groups/{id}/members. Para contornar isso, recomendamos que você remova o usuário dos proprietários e membros, espere 10 segundos e adicione-os novamente aos membros.

Ao adicionar e remover membros e proprietários, não coloque chaves { } ao redor da ID.

| Velocidade | Sintaxe |
| ------ | ----- |
| Rápida | `https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref` |
| Lento | `https://graph.microsoft.com/beta/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref` |

Da mesma forma, se o `userId` na URL ou no conteúdo for expresso como um UPN, e não como um GUID, o desempenho será mais lento.

| Velocidade | Sintaxe |
| ------ | ----- |
| Rápida | 48d31887-5fad-4d73-a9f5-3c356e68a038 |
| Lento | vitor@example.com |

Quando o caminho mais lento é executado, se um membro ou membro da equipe atual estiver conectado ao aplicativo/site do Microsoft Teams, a alteração será refletida em uma hora.
Se nenhum desses usuários estiver conectado ao aplicativo/site do Microsoft Teams, a alteração não será refletida até uma hora depois que um deles se conectar.

> [!Note]
> Os convidados do locatário sempre são processados pelo caminho lento.

## <a name="polling-requirements"></a>Requisitos de sondagem

Se seu aplicativo sonda para ver se um recurso foi alterado, você só poderá fazer isso uma vez por dia. ([teamsAsyncOperation](teamsasyncoperation.md) é uma exceção no sentido de que é foi desenvolvida para ser sondada frequentemente.) Se você precisar saber sobre mudanças com mais frequência que esta, você deve [criar uma assinatura](../api/subscription-post-subscriptions.md) para esse recurso e receber notificações de alteração (webhooks). Caso não encontre suporte para o tipo de assinatura necessária, recomendamos que você faça comentários por meio do [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests?category_id=359626). 

Ao pesquisar novas mensagens, você deve especificar um intervalo de datas onde isso for possível.  Para obter detalhes, consulte [obter mensagens de canal delta](../api/chatmessage-delta.md).

As sondagem está executando uma operação OBTER em um recurso repetidamente para ver se o recurso foi alterado. Você tem permissão para obter o mesmo recurso várias vezes por dia, desde que não seja uma sondagem. Por exemplo, está tudo bem se você usar OBTER /me/joinedTeams toda vez que o usuário visita/atualiza sua página da web, mas não é certo usar OBTER /me/joinedTeams em um loop a cada 30 segundos para atualizar essa página da web.

Os aplicativos que não seguem esses requisitos de sondagem serão considerados violações de [termos de uso das APIs da Microsoft](/legal/microsoft-apis/terms-of-use). A violação destes Termos da API pode resultar [suspensão](/graph/throttling)ou no cancelamento do uso das APIs da Microsoft.

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="see-also"></a>Confira também

- [Visão geral da API do Microsoft Teams](/graph/teams-concept-overview)
- Exemplo de código: [Linhas Aéreas Contoso](https://github.com/microsoftgraph/contoso-airlines-teams-sample), [mini exemplos C#](https://github.com/microsoftgraph/csharp-teams-sample-graph)
