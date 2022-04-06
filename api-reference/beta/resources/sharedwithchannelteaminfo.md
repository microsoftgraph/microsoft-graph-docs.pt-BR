---
title: Tipo de recurso sharedWithChannelTeamInfo
description: Representa uma equipe que é compartilhada com um canal.
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e26bc3db8359ccb560e2922dcb6c8b8328fc2b74
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685331"
---
# <a name="sharedwithchannelteaminfo-resource-type"></a>Tipo de recurso sharedWithChannelTeamInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma [equipe](team.md) que é compartilhada com um canal. Uma [equipe](team.md) pode ser compartilhada com vários canais.


Herda de [teamInfo](../resources/teaminfo.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-list.md)|[Coleção sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Obtenha uma lista dos [objetos sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) e suas propriedades.|
|[Obter sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-get.md)|[sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Leia as propriedades e as relações de um [objeto sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) .|
|[Excluir sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-delete.md)|Nenhuma|[Exclua um objeto sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md).|
|[Listar allowedMembers](../api/sharedwithchannelteaminfo-list-allowedmembers.md)|[conversationMember](../resources/conversationmember.md)coleção|Obtenha a lista de membros da equipe que têm acesso ao canal compartilhado.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome da equipe. Herdado de [teamInfo](../resources/teaminfo.md).|
|isHostTeam|Booliano|Indica se a [equipe](team.md) é o host do [canal](channel.md).|
|tenantId|String|A ID do locatário Azure Active Directory usuário. Herdado de [teamInfo](../resources/teaminfo.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|allowedMembers|coleção [conversationMember](../resources/conversationmember.md)|Uma coleção de membros da equipe que têm acesso ao canal compartilhado.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedWithChannelTeamInfo",
  "baseType": "microsoft.graph.teamInfo",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedWithChannelTeamInfo",
  "displayName": "String",
  "id": "String (identifier)",
  "isHostTeam": "Boolean",
  "tenantId": "String"
}
```

