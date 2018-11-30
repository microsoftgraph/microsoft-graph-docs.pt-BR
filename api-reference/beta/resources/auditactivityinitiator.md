---
title: tipo de recurso de auditActivityInitiator
description: O objeto resource que inicia a atividade de identidade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)
ms.openlocfilehash: 834b39f67a9a3a251c61f15d3b1fa8aa964870e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037865"
---
# <a name="auditactivityinitiator-resource-type"></a>tipo de recurso de auditActivityInitiator
O objeto resource que inicia a atividade de identidade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|app|[appIdentity](appidentity.md)|Se o recurso iniciando a atividade for um aplicativo, esta propriedade indica o aplicativo todas as informações como appId, relacionadas ao nome, servicePrincipalId, nome.|
|user|[userIdentity](useridentity.md)|Se o recurso iniciando a atividade for um usuário, esta propriedade indica todos os usuários informações como userId, nome, UserPrinicpalName relacionadas.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}-->

```json
{
  "app": {"@odata.type": "microsoft.graph.appIdentity"},
  "user": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditActivityInitiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->