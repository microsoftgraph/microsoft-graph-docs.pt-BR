---
title: tipo de recurso de equipe
description: 'Uma equipe Teams da Microsoft é uma coleção de canais. '
author: nkramer
ms.openlocfilehash: 0ed654bf4c8d627dd9466f9263b121f85800b853
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345476"
---
# <a name="team-resource-type"></a>tipo de recurso de equipe

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma equipe Teams da Microsoft é uma coleção de [canais](channel.md). Um canal representa um tópico e, portanto, um isolamento lógico discussão, dentro de uma equipe.

Cada equipe é associado um [grupo](../resources/group.md).
O grupo tem a mesma identificação que a equipe - por exemplo, /groups/ {id} / equipe é igual ao /teams/ {id}.
Para obter mais informações sobre como trabalhar com grupos e membros de equipes, consulte [Use a API do Microsoft Graph REST para trabalhar com as equipes da Microsoft](teams-api-overview.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar equipe](../api/team-post.md) | [teamsAsyncOperation](teamsasyncoperation.md) | Crie uma equipe do zero. |
|[Criar equipe a partir de grupo](../api/team-put-teams.md) | [equipe](team.md) | Criar um novo equipe ou adicione uma equipe a um grupo existente.|
|[Obtenha a equipe](../api/team-get.md) | [equipe](team.md) | Recupere as propriedades e relacionamentos da equipe especificado.|
|[Equipe de atualização](../api/team-update.md) | [equipe](team.md) |Atualize as propriedades da equipe especificado. |
|[Excluir equipe](/graph/api/group-delete?view=graph-rest-1.0) | Nenhum |Exclua a equipe e seu grupo associado. |
|[Equipe de clone](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Copie a equipe e seu grupo associado. |
|[Equipe de arquivo morto](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Colocar a equipe em um estado somente leitura. |
|[Equipe de unarchive](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Restaure a equipe em um estado de leitura / gravação. |
|[Listar suas equipes](../api/user-list-joinedteams.md) | coleção de [equipe](team.md) | Liste as equipes que você é um membro de. |
|[Liste todas as equipes](/graph/teams-list-all-teams) | Coleção [group](group.md) | Liste todos os grupos que possuem equipes. |
|[Publicar aplicativos à sua organização](../resources/teamsapp.md)| [teamsApp](../resources/teamsapp.md) | Crie aplicativos de equipes visível somente para sua organização. |
|[Adicionar o aplicativo à equipe](../api/teamsappinstallation-add.md) | [teamsappinstallation](teamsappinstallation.md) | Adiciona (instala) um aplicativo para uma equipe.|
|[Adicionar guia ao canal](../api/teamstab-add.md) | [teamsTab](../resources/teamstab.md) | Adiciona (instala) uma guia ao canal da equipe.|
|[Lista de mensagens de canal](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | [Obter mensagens em um canal](../api/channel-list-messages.md) |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:---------------|:--------|:----------|
|displayName|string| O nome da equipe. |
|description|string| Uma descrição opcional para a equipe. |
|classificação|string| Um rótulo opcional. Normalmente, descreve a sensibilidade de dados ou de negócios da equipe. Deve corresponder a um conjunto pré-configurado no diretório de locatário. |
|especialização|[teamSpecialization](teamspecialization.md)| Opcional. Indica se a equipe destina-se de um caso de uso específico.  Especialização cada equipe tem acesso aos comportamentos exclusivos e experiências destinadas ao seu caso de uso. |
|visibilidade|[teamVisibilityType](teamvisibilitytype.md)| A visibilidade de um o grupo e da equipe. Por padrão, público. |
|funSettings|[teamFunSettings](teamfunsettings.md) |Configurações para configurar o uso de Giphy, memes e adesivos na equipe de.|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |Configurações para configurar se os convidados podem criar, atualizar ou excluir canais na equipe de.|
|isArchived|Boolean|Se essa equipe está em modo somente leitura. |
|memberSettings|[teamMemberSettings](teammembersettings.md) |Configurações para configurar se os membros podem realizar determinadas ações, por exemplo, criam canais e adicionar bots, na equipe de.|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |Configurações para configurar mensagens e menções na equipe de.|
|webUrl|cadeia de caracteres (somente leitura) | Um hiperlink que irão para a equipe no cliente do Microsoft Teams. Esta é a URL que você obtém quando você uma equipe no cliente do Microsoft Teams do mouse em e selecione o **link para a equipe de obter**. Essa URL deve ser tratado como um blob opaco e não analisado. |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:---------------|:--------|:----------|
|Aplicativos|coleção [teamsApp](teamsapp.md)| (Obsoleto) Os aplicativos instalados nesse conjunto.|
|canais|coleção de [canal](channel.md)|A coleção de canais & associadas à equipe de mensagens.|
|installedApps|coleção [teamsAppInstallation](teamsappinstallation.md)|Os aplicativos instalados nesse conjunto.|
|owners|[user](user.md)| A lista de proprietários dessa equipe. |
|modelo|[teamsTemplate](teamstemplate.md)| O modelo a partir do qual essa equipe foi criada. |

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
  "isArchived": false,
  "webUrl": "https://...longUrl..."
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>Confira também
- [Criando um grupo com uma equipe](/graph/teams-create-group-and-team)
- [Visão geral da API de equipes](teams-api-overview.md)
