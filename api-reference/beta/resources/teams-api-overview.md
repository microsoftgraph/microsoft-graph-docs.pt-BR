---
title: Usar o Microsoft Graph API para trabalhar com o Microsoft Teams
description: O Microsoft Teams é um espaço de trabalho baseado em chat no Office 365 que fornece acesso interno a calendários, arquivos, anotações do OneNote, planos do Planner e muito mais.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: 34f5186e9933f5edcd8a91b1cb95b21b6deb4a50
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353900"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Usar o Microsoft Graph API para trabalhar com o Microsoft Teams

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Microsoft Teams é um espaço de trabalho baseado em chat no Office 365 que fornece acesso interno a calendários específicos, arquivos, anotações do OneNote, planos do Planner, cronogramas de turno e muito mais.

## <a name="key-resources-in-microsoft-teams"></a>Principais recursos no Microsoft Teams (visualização)

| Resource | Métodos |
|:---------------|:--------|
|[team](../resources/team.md)| [Listar suas equipes](../api/user-list-joinedteams.md), [listar todas as equipes](/graph/teams-list-all-teams), [criar](../api/team-put-teams.md), [ler](../api/team-get.md), [atualizar](../api/team-update.md), [excluir](/graph/api/group-delete?view=graph-rest-1.0), [clonar](../api/team-clone.md), [arquivar](../api/team-archive.md), [cancelar o arquivamento](../api/team-unarchive.md) |
|[group](../resources/group.md)| [Adicionar membro](../api/group-post-members.md),  [remover membro](../api/group-delete-members.md), [adicionar proprietário](../api/group-post-owners.md),  [remover proprietário](../api/group-delete-owners.md), [obter arquivos](drive.md), [obter bloco de anotações](/graph/api/resources/notebook?view=graph-rest-1.0), [obter planos](plannergroup.md), [obter calendário](event.md) |
|[channel](../resources/channel.md)|[Listar](../api/channel-list.md), [criar](../api/channel-post.md), [ler](../api/channel-get.md), [atualizar](../api/channel-patch.md), [excluir](../api/channel-delete.md)|
|[teamsTab](../resources/teamstab.md) |[Listar](../api/teamstab-list.md), [criar](../api/teamstab-add.md), [ler](../api/teamstab-get.md), [atualizar](../api/teamstab-update.md), [excluir](../api/teamstab-delete.md) |
|[teamsApp](../resources/teamsapp.md)|[Listar](../api/teamsapp-list.md), [publicar](../api/teamsapp-publish.md), [atualizar](../api/teamsapp-update.md), [remover](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [Listar](../api/teamsappinstallation-list.md), [instalar](../api/teamsappinstallation-add.md), [atualizar](../api/teamsappinstallation-delete.md), [remover](../api/teamsappinstallation-delete.md) |
|[chatMessage](../resources/chatmessage.md) (visualização)| [Lista](../api/channel-list-messages.md), [enviar](../api/channel-post-messages.md), [ler](/graph/api/channel-get-message?view=graph-rest-beta) |
|[Chamada](/graph/api/resources/communications-api-overview.md) (visualização) | [Responder](/graph/api/call-answer?view=graph-rest-beta), [rejeitar](/graph/api/call-reject?view=graph-rest-beta), [redirecionar](/graph/api/call-redirect?view=graph-rest-beta), [ativar mudo](/graph/api/call-mute?view=graph-rest-beta), [desfazer ativar mudo](/graph/api/call-unmute?view=graph-rest-beta), [atualizar metadados](/graph/api/call-updatemetadata?view=graph-rest-beta), [alterar a função de compartilhamento de tela](/graph/api/call-changescreensharingrole?view=graph-rest-beta), [listar participantes](/graph/api/call-list-participants?view=graph-rest-beta), [convidar participantes](/graph/api/participant-invite?view=graph-rest-beta), [ativar mudo para todos os participantes](/graph/api/participant-muteall?view=graph-rest-beta) |
|[cronograma](/graph/api/resources/schedule?view=graph-rest-beta) (visualização)| [Criar ou substituir](/graph/api/team-put-schedule?view=graph-rest-beta), [obter](/graph/api/schedule-get?view=graph-rest-beta), [compartilhar](/graph/api/schedule-share?view=graph-rest-beta) |
|[schedulingGroup](/graph/api/resources/schedulinggroup?view=graph-rest-beta) visualização| [Criar](/graph/api/schedule-post-schedulinggroups?view=graph-rest-beta), [Listar](/graph/api/schedule-list-schedulinggroups?view=graph-rest-beta), [Obter](/graph/api/schedulinggroup-get?view=graph-rest-beta), [Substituir](/graph/api/schedulinggroup-put?view=graph-rest-beta), [Excluir](/graph/api/schedulinggroup-delete?view=graph-rest-beta) |
|[turno](/graph/api/resources/shift?view=graph-rest-beta) (visualização)| [Criar](/graph/api/schedule-post-shifts?view=graph-rest-beta), [Listar](/graph/api/schedule-list-shifts?view=graph-rest-beta), [Obter](/graph/api/shift-get?view=graph-rest-beta), [Substituir](/graph/api/shift-put?view=graph-rest-beta), [Excluir](/graph/api/shift-delete?view=graph-rest-beta) |
|[Folga](/graph/api/resources/timeoff?view=graph-rest-beta) (visualização)| [Criar](/graph/api/schedule-post-timesoff?view=graph-rest-beta), [Listar](/graph/api/schedule-list-timesoff?view=graph-rest-beta), [Obter](/graph/api/timeoff-get?view=graph-rest-beta), [Substituir](/graph/api/timeoff-put?view=graph-rest-beta), [Excluir](/graph/api/timeoff-delete?view=graph-rest-beta) |
|[timeOffReason](/graph/api/resources/timeoffreason?view=graph-rest-beta) (visualização)| [Criar](/graph/api/schedule-post-timeoffreasons?view=graph-rest-beta), [Listar](/graph/api/schedule-list-timeoffreasons?view=graph-rest-beta), [Obter](/graph/api/timeoffreason-get?view=graph-rest-beta), [Substituir](/graph/api/timeoffreason-put?view=graph-rest-beta), [Excluir](/graph/api/timeoffreason-delete?view=graph-rest-beta) |

## <a name="microsoft-teams-limits"></a>Limites do Microsoft Teams

As limitações de desempenho e de capacidade testadas do Microsoft Teams estão documentadas nas [especificações e limites do Microsoft Teams](/microsoftteams/limits-specifications-teams).
Esses limites aplicam-se diretamente ao usar o Microsoft Teams ou usar as APIs do Microsoft Graph.
Como todas as equipes têm um grupo correspondente, e cada grupo é um objeto de diretório, limites no [número de grupos](/microsoft-365/admin/create-groups/office-365-groups#group-limits) e o [número de objetos de diretório ("recursos")](/azure/active-directory/users-groups-roles/directory-service-limits-restrictions) também podem ser levados em consideração. 

Os arquivos dentro de canais são armazenados no SharePoint. [os limites do SharePoint Online](/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits) se aplicam.

Confira também [redução dos limites dos serviços do Microsoft Teams](/graph/throttling).

## <a name="teams-and-groups"></a>Equipes e grupos

Na Microsoft Graph, o Microsoft Teams é representado por um recurso de [grupo](../resources/group.md). Os grupos do Microsoft Teams e Office 365 atendem às várias necessidades de colaboração em grupo. Quase todos os recursos baseados em grupo se aplicam aos grupos do Microsoft Teams e do Office 365, como calendário de grupo, arquivos, anotações, fotos, planos e assim por diante. A principal diferença entre uma [equipe](team.md) e um grupo do Office 365 é o modo de comunicação entre os membros. Os membros da equipe se comunicam por meio de chat persistente no contexto de uma equipe específica. Os membros do grupo do Office 365 se comunicam por conversas em grupo, que são conversas por email que ocorrem no contexto de um grupo no Outlook.

Qualquer grupo que tenha uma equipe possui uma propriedade **resourceProvisioningOptions** que contém "Team".

>**Observação:** a propriedade **Group.resourceProvisioningOptions** pode ser alterada.
Não adicione ou remova "Team" dessa coleção; caso contrário, você obterá resultados incorretos ao listar todas as equipes.

Veja a seguir as diferenças no nível da API entre equipes e grupos:

- O chat persistente está disponível apenas para o Microsoft Teams. Esse recurso é representado hierarquicamente pelos recursos [channel](../resources/channel.md) e [chatMessage](../resources/chatmessage.md).
- As conversas em grupo estão disponíveis apenas para grupos do Office 365. Esse recurso é representado hierarquicamente pelos recursos [conversation](../resources/conversation.md), [conversationThread](../resources/conversationthread.md) e [post](../resources/post.md). 
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
| Rápida | https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref |
| Lento | https://graph.microsoft.com/beta/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref |

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

Ao pesquisar novas mensagens, você deve especificar um intervalo de datas onde isso for possível.  Para obter detalhes, consulte [obter mensagens de canal delta](/graph/api/chatmessage-delta?view=graph-rest-beta).

As sondagem está executando uma operação OBTER em um recurso repetidamente para ver se o recurso foi alterado. Você tem permissão para obter o mesmo recurso várias vezes por dia, desde que não seja uma sondagem. Por exemplo, está tudo bem se você usar OBTER /me/joinedTeams toda vez que o usuário visita/atualiza sua página da web, mas não é certo usar OBTER /me/joinedTeams em um loop a cada 30 segundos para atualizar essa página da web.

Os aplicativos que não seguem esses requisitos de sondagem serão considerados violações de [termos de uso das APIs da Microsoft](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use). A violação destes Termos da API pode resultar [suspensão](/graph/throttling)ou no cancelamento do uso das APIs da Microsoft.

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="see-also"></a>Confira também

[Visão geral da API do Microsoft Teams](/graph/teams-concept-overview)
