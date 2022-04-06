---
title: Tipo de recurso associatedTeamInfo
description: Representa uma equipe associada a um usuário.
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2e3c8c83d10d5c15595edf9aef8f0b3b50e661e4
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685408"
---
# <a name="associatedteaminfo-resource-type"></a>Tipo de recurso associatedTeamInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma [equipe](team.md) associada a um [usuário](../resources/user.md). Atualmente, um [usuário pode](../resources/user.md) ser associado a uma [equipe](../resources/team.md) de duas maneiras diferentes:
* Um [usuário](../resources/user.md) pode ser um membro direto de uma [equipe](../resources/team.md).
* Um [usuário](../resources/user.md) pode ser membro de um canal [compartilhado](../resources/channel.md) hospedado dentro de uma [equipe](../resources/team.md).



Herda de [teamInfo](../resources/teaminfo.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar associatedTeamInfo](../api/associatedteaminfo-list.md)|[coleção associatedTeamInfo](../resources/associatedteaminfo.md)|Obtenha a lista de [objetos AssociatedTeamInfo](../resources/associatedteaminfo.md) e suas propriedades.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome da equipe. Herdado de [teamInfo](../resources/teaminfo.md).|
|tenantId|String|A ID do locatário Azure Active Directory usuário. Herdado de [teamInfo](../resources/teaminfo.md).|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.associatedTeamInfo",
  "baseType": "microsoft.graph.teamInfo",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.associatedTeamInfo",
  "displayName": "String",
  "id": "String (identifier)",
  "tenantId": "String"
}
```

## <a name="see-also"></a>Confira também
- [Obter equipe](../api/team-get.md)