---
title: Tipo de recurso sharedWithChannelTeamInfo
description: Representa uma equipe que é compartilhada com um canal.
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 15f6e3138d24bf93a2546be404c21e6bcf4b6daa
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060997"
---
# <a name="sharedwithchannelteaminfo-resource-type"></a>Tipo de recurso sharedWithChannelTeamInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma informação para uma [equipe](team.md) com a qual um canal é compartilhado. Uma [equipe](team.md) pode ser compartilhada em vários canais.


Herda de [teamInfo](../resources/teaminfo.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-list.md)|Coleção [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Obtenha uma lista dos objetos [sharedWithChannelTeamInfo ](../resources/sharedwithchannelteaminfo.md) e suas propriedades.|
|[Obter sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-get.md)|[sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Leia sobre as propriedades e relações de um objeto [sharedWithChannelTeamInfo ](../resources/sharedwithchannelteaminfo.md).|
|[Excluir sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-delete.md)|Nenhum|Excluir um objeto [sharedWithChannelTeamInfo ](../resources/sharedwithchannelteaminfo.md).|
|[Listar allowedMembers](../api/sharedwithchannelteaminfo-list-allowedmembers.md)|[conversationMember](../resources/conversationmember.md)coleção|Obtenha a lista de membros da equipe que têm acesso ao canal compartilhado.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome da equipe. Herdado de [teamInfo](../resources/teaminfo.md).|
|isHostTeam|Boolean|Indica se a [equipe](team.md) é o host do [canal](channel.md).|
|tenantId|String|A ID do locatário do Active Directory do Azure. Herdado de [teamInfo](../resources/teaminfo.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|membrosPermitidos|[conversationMember](../resources/conversationmember.md)coleção|Uma coleção de membros da equipe que têm acesso ao canal compartilhado.|


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

