---
title: tipo de recurso de equipe
description: 'No Microsoft Teams, uma equipe é um conjunto de canais. '
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 85315d43b1de42e74b83d0ba9664ebfdb7847258
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908513"
---
# <a name="team-resource-type"></a>tipo de recurso de equipe

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No Microsoft Teams, uma equipe é um conjunto de objetos de [canal](channel.md). Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe.

Cada equipe está associada a um [grupo](../resources/group.md). O grupo tem a mesma ID da equipe, por exemplo, `/groups/{id}/team` é o mesmo `/teams/{id}`. Confira mais informações sobre como trabalhar com grupos e membros em equipes, confira [Usar a API REST do Microsoft Graph para trabalhar com o Microsoft Teams](teams-api-overview.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar equipe](../api/team-post.md) | [teamsAsyncOperation](teamsasyncoperation.md) | Crie uma equipe do zero. |
|[Criar equipe a partir do grupo](../api/team-put-teams.md) | [team](team.md) | Crie uma nova equipe ou adicione uma equipe a um grupo existente.|
|[Obter equipe](../api/team-get.md) | [team](team.md) | Recupere as propriedades e relações da equipe especificada.|
|[Atualizar equipe](../api/team-update.md) | [team](team.md) |Atualize as propriedades da equipe especificada. |
|[Excluir equipe](/graph/api/group-delete?view=graph-rest-1.0) | Nenhum |Exclua a equipe e o grupo associado. |
|[Clonar equipe](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Copie a equipe e o grupo associado. |
|[Arquivar equipe](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Coloque a equipe em um estado somente leitura. |
|[Desarquivar equipe](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Restaure a equipe com um estado de leitura e gravação. |
|[Listar suas equipes](../api/user-list-joinedteams.md) | Coleção [team](team.md) | Liste as equipes das quais você é membro. |
|[Listar todas as equipes](/graph/teams-list-all-teams) | Coleção [group](group.md) | Liste todos os grupos que têm equipes. |
|[Publicar aplicativos para sua organização](../resources/teamsapp.md)| [teamsApp](../resources/teamsapp.md) | Crie aplicativos do Teams que apenas sua organização possa ver. |
|[Adicionar aplicativo à equipe](../api/teamsappinstallation-add.md) | [teamsAppInstallation](teamsappinstallation.md) | Adiciona (instala) um aplicativo a uma equipe.|
|[Adicionar uma guia ao canal](../api/teamstab-add.md) | [teamsTab](../resources/teamstab.md) | Adiciona (instala) uma guia ao canal de uma equipe.|
|[Listar mensagens do canal](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | [Obter mensagens em um canal](../api/channel-list-messages.md) |
|[Criar uma chatMessage em um canal](../api/channel-post-messages.md)  | [chatMessage](../resources/chatmessage.md) | Envie uma mensagem para um canal. |
|[Criar uma resposta chatMessage em um canal](../api/channel-post-messagereply.md) | [chatMessage](../resources/chatmessage.md) | Responda a uma mensagem em um canal. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|displayName|string| O nome da equipe. |
|description|string| Uma descrição opcional para a equipe. |
|classificação|string| Um rótulo opcional. Normalmente descreve a confidencialidade da empresa ou dos dados da equipe. Deve coincidir com um dos conjuntos predefinidos no diretório do locatário. |
|specialization|[teamSpecialization](teamspecialization.md)| Opcional. Indica se a equipe destina-se a um caso de uso específico.  Cada especialização de equipe tem acesso a comportamentos e experiências exclusivos direcionados ao seu caso de uso. |
|visibility|[teamVisibilityType](teamvisibilitytype.md)| A visibilidade de um grupo e equipe. O padrão é Público. |
|funSettings|[teamFunSettings](teamfunsettings.md) |Configurações que definem o uso de Giphy, memes e figurinhas na equipe.|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |Configurações que definem se os convidados podem criar, atualizar ou excluir canais na equipe.|
|internalId | string | Uma ID exclusiva da equipe, que foi usada em alguns locais, como o log de auditoria da [API da Atividade de Gestão do Office 365](https://docs.microsoft.com/pt-BR/office/office-365-management-api/office-365-management-activity-api-reference). |
|isArchived|Booliano|Se essa equipe está no modo somente leitura. |
|memberSettings|[teamMemberSettings](teammembersettings.md) |Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |Configurações para definir a mensagens e menções na equipe.|
|discoverySettings|[teamDiscoverySettings](teamdiscoverysettings.md) |Configurações de capacidade de descoberta da equipe por outras pessoas.|
|webUrl|cadeia de caracteres (somente leitura) | Um hiperlink que será enviado à equipe no cliente do Microsoft Teams. Esta é a URL que você recebe ao clicar com o botão direito do mouse em uma equipe no cliente do Microsoft Teams e escolher **Obter o link para a equipe**. Essa URL deve ser tratada como um blob opaco e não analisado. |

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|apps|Coleção [teamsApp](teamsapp.md)| (Obsoleto) Os aplicativos instalados nessa equipe.|
|channels|Coleção [channel](channel.md)|A coleção de canais e mensagens associadas à equipe.|
|installedApps|Coleção [teamsAppInstallation](teamsappinstallation.md)|Os aplicativos instalados nessa equipe.|
|owners|[user](user.md)| A lista de proprietários desta equipe. Atualmente, ao criar uma equipe usando permissões de aplicativo, exatamente um proprietário deve ser especificado. Ao usar permissões delegadas pelo usuário, nenhum proprietário pode ser especificado (o usuário atual é o proprietário). O proprietário deve ser especificado como um objeto ID (GUID), não um UPN. |
|operations|Coleção [teamsAsyncOperation](teamsasyncoperation.md)| As operações assíncronas que foram executadas ou estão em execução nesta equipe. | 
|primaryChannel|[canal](channel.md)|O canal principal associado à equipe.|
|Cronograma|[Cronograma](schedule.md)| Cronograma de turno para essa equipe.|
|template|[teamsTemplate](teamstemplate.md)| O modelo usado para criar essa equipe. Confira os [modelos disponíveis](https://docs.microsoft.com/pt-BR/MicrosoftTeams/get-started-with-teams-templates). |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "guestSettings": {"@odata.type": "microsoft.graph.teamGuestSettings"},
  "memberSettings": {"@odata.type": "microsoft.graph.teamMemberSettings"},
  "messagingSettings": {"@odata.type": "microsoft.graph.teamMessagingSettings"},
  "funSettings": {"@odata.type": "microsoft.graph.teamFunSettings"},
  "discoverySettings": {"@odata.type": "microsoft.graph.teamDiscoverySettings"},
  "internalId": "string",
  "isArchived": false,
  "webUrl": "string (URL)",
  "displayName": "string",
  "description": "string",
  "classification": "string",
  "specialization": "string",
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a>Confira também

- [Como criar um grupo com uma equipe](/graph/teams-create-group-and-team)
- [Visão geral da API do Teams](teams-api-overview.md)
