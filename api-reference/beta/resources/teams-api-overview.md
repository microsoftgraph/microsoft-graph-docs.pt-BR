---
title: Usar o Microsoft Graph API para trabalhar com o Microsoft Teams
description: O Microsoft Teams é um espaço de trabalho baseado em chat no Microsoft 365 que fornece acesso interno a calendários, arquivos, anotações do OneNote, planos do Planner e muito mais.
ms.localizationpriority: high
author: nkramer
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: fe1d1da1ddf03a3b25a206c380f6ce9b6886650e
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883081"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Usar o Microsoft Graph API para trabalhar com o Microsoft Teams

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Microsoft Teams é um espaço de trabalho baseado em chat no Microsoft 365 que fornece acesso interno a calendários, arquivos, anotações do OneNote, planos do Planner e muito mais.

## <a name="key-resources-in-microsoft-teams"></a>Principais recursos no Microsoft Teams (visualização)

| Resource | Métodos |
|:---------------|:--------|
|[team](../resources/team.md)| [Listar suas equipes](../api/user-list-joinedteams.md), [listar todas as equipes](/graph/teams-list-all-teams), [listar as equipes associadas ](../api/associatedteaminfo-list.md), [criar](../api/team-put-teams.md), [ler](../api/team-get.md), [atualizar](../api/team-update.md), [excluir](../api/group-delete.md), [clonar](../api/team-clone.md), [arquivar](../api/team-archive.md), [ desarquivar](../api/team-unarchive.md) |
|[chamada](../resources/call.md)| [Responder](../api/call-answer.md), [rejeitar](../api/call-reject.md), [redirecionar](../api/call-redirect.md), [silenciar](../api/call-mute.md), [não silenciar](../api/call-unmute.md), [alterar função de compartilhamento de tela](../api/call-changescreensharingrole.md), [lista de participantes](../api/call-list-participants.md), [convidar participantes](../api/participant-invite.md), [silenciar todos os participantes](../api/participant-muteall.md) |
|[canal](../resources/channel.md)|[Listar](../api/channel-list.md), [criar](../api/channel-post.md), [obter](../api/channel-get.md), [atualizar](../api/channel-patch.md), [excluir](../api/channel-delete.md)|
|[chat](../resources/chat.md)| [Listar](../api/chat-list.md), [ler](../api/chat-get.md)
|[chatMessage](../resources/chatmessage.md)| [Listar no canal](../api/channel-list-messages.md), [listar no chat](../api/chat-list-messages.md), [enviar](../api/chatmessage-post.md), [ler no canal](../api/chatmessage-get.md), [ler no chat](../api/chatmessage-get.md)|
|[group](../resources/group.md)| [Adicionar membro](../api/group-post-members.md),  [remover membro](../api/group-delete-members.md), [adicionar proprietário](../api/group-post-owners.md),  [remover proprietário](../api/group-delete-owners.md), [obter arquivos](drive.md), [obter bloco de anotações](../resources/notebook.md), [obter planos](plannergroup.md), [obter calendário](event.md) |
|[learningContent](learningcontent.md) | [Listar](../api/learningprovider-list-learningcontents.md), [Obter](../api/learningcontent-get.md), [Atualizar](../api/learningcontent-update.md), [Excluir](../api/learningprovider-delete-learningcontents.md) |
|[learningProvider](learningprovider.md) | [Listar](../api/employeeexperience-list-learningproviders.md), [Criar](../api/employeeexperience-post-learningproviders.md), [Obter](../api/learningprovider-get.md), [Atualizar](../api/learningprovider-update.md), [Excluir](../api/employeeexperience-delete-learningproviders.md) |
|[cronograma](../resources/schedule.md)| [Criar ou substituir](../api/team-put-schedule.md), [obter](../api/schedule-get.md), [compartilhar](../api/schedule-share.md) |
|[schedulingGroup](../resources/schedulinggroup.md)| [Criar](../api/schedule-post-schedulinggroups.md), [listar](../api/schedule-list-schedulinggroups.md), [obter](../api/schedulinggroup-get.md), [substituir](../api/schedulinggroup-put.md), [excluir](../api/schedulinggroup-delete.md) |
|[shift](../resources/shift.md)| [Criar](../api/schedule-post-shifts.md), [listar](../api/schedule-list-shifts.md), [obter](../api/shift-get.md), [substituir](../api/shift-put.md), [excluir](../api/shift-delete.md) |
|[marcar](../resources/teamworkTag.md)|[Listar](../api/teamworkTag-list.md), [criar](../api/teamworkTag-post.md), [obter](../api/teamworkTag-get.md), [atualizar](../api/teamworkTag-update.md), [excluir](../api/teamworkTag-delete.md)|
|[tagMember](../resources/teamworkTagMember.md)|[Listar](../api/teamworkTagMember-list.md), [criar](../api/teamworkTagMember-post.md), [obter](../api/teamworkTagMember-get.md), [excluir](../api/teamworkTagMember-delete.md)|
|[teamsApp](../resources/teamsapp.md)|[Listar](../api/appcatalogs-list-teamsapps.md), [publicar](../api/teamsapp-publish.md), [atualizar](../api/teamsapp-update.md), [remover](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [Listar](../api/team-list-installedapps.md), [instalar](../api/team-post-installedapps.md), [atualizar](../api/team-delete-installedapps.md), [remover](../api/team-delete-installedapps.md) |
|[teamsTab](../resources/teamstab.md) |[Listar](../api/channel-list-tabs.md), [criar](../api/channel-post-tabs.md), [ler](../api/channel-get-tabs.md), [atualizar](../api/channel-patch-tabs.md), [excluir](../api/channel-delete-tabs.md) |
|[timeOff](../resources/timeoff.md)| [Criar](../api/schedule-post-timesoff.md), [listar](../api/schedule-list-timesoff.md), [obter](../api/timeoff-get.md), [substituir](../api/timeoff-put.md), [excluir](../api/timeoff-delete.md) |
|[timeOffReason](../resources/timeoffreason.md)| [Criar](../api/schedule-post-timeoffreasons.md), [listar](../api/schedule-list-timeoffreasons.md), [obter](../api/timeoffreason-get.md), [substituir](../api/timeoffreason-put.md), [excluir](../api/timeoffreason-delete.md) |

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

| Caso de uso      | Verbo      | URL |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Adicionar membro](../api/team-post-members.md) | POST      | /teams/{team-id}/members  |
| [Remover membro](../api/team-delete-members.md)    | DELETE    | /teams/{team-id}/members/{membership-id} |
| [Atualizar a função do membro](../api/team-update-members.md) | PATCH | /teams/{team-id}/members/{membership-id} |
| [Atualizar equipe](../api/team-update.md)  | PATCH     | /teams/{team-id} |

## <a name="polling-requirements"></a>Requisitos de sondagem

Se seu aplicativo sonda para ver se um recurso foi alterado, você só poderá fazer isso uma vez por dia.
([teamsAsyncOperation](teamsasyncoperation.md) é uma exceção no sentido de que é foi desenvolvida para ser sondada frequentemente.) Se você precisar saber sobre mudanças com mais frequência que esta, você deve [criar uma assinatura](../api/subscription-post-subscriptions.md) para esse recurso e receber notificações de alteração (webhooks).
Caso não encontre suporte para o tipo de assinatura necessária, recomendamos que você faça comentários por meio do [Fórum de ideias da Plataforma para Desenvolvedores do Microsoft 365 ](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).

Ao pesquisar novas mensagens, você deve especificar um intervalo de datas onde isso for possível.  Para obter detalhes, consulte [obter mensagens de canal delta](../api/chatmessage-delta.md).

As sondagem está executando uma operação OBTER em um recurso repetidamente para ver se o recurso foi alterado.
Você tem permissão para obter o mesmo recurso várias vezes por dia, desde que não seja uma sondagem.
Por exemplo, está tudo bem se você usar OBTER /me/joinedTeams toda vez que o usuário visita/atualiza sua página da web, mas não é certo usar OBTER /me/joinedTeams em um loop a cada 30 segundos para atualizar essa página da web.

Os aplicativos que não seguem esses requisitos de sondagem serão considerados violações de [termos de uso das APIs da Microsoft](/legal/microsoft-apis/terms-of-use). A violação destes Termos da API pode resultar [suspensão](/graph/throttling)ou no cancelamento do uso das APIs da Microsoft.

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="see-also"></a>Confira também

- [Visão geral da API do Microsoft Teams](/graph/teams-concept-overview)
- Exemplo de código: [Linhas Aéreas Contoso](https://github.com/microsoftgraph/contoso-airlines-teams-sample), [mini exemplos C#](https://github.com/microsoftgraph/csharp-teams-sample-graph)
