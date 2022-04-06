---
title: Tipo de recurso teamInfo
description: Representa uma equipe com informações básicas.
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0e2d683428dae15a0b51989906dbb9ecac16b945
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685338"
---
# <a name="teaminfo-resource-type"></a>Tipo de recurso teamInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma [equipe](team.md) com informações básicas.

Tipo base [de associatedTeamInfo](associatedteaminfo.md) e [sharedWithChannelTeamInfo](sharedwithchannelteaminfo.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome da equipe.|
|tenantId|String|A ID do locatário Azure Active Directory usuário.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamInfo",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamInfo",
  "displayName": "String",
  "id": "String (identifier)",
  "tenantId": "String"
}
```
