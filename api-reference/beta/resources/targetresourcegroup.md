---
title: tipo de recurso de targetResourceGroup
description: 'Indica o tipo de grupo que foi afetado devido a atividade de auditoria. Inclui valores como os grupos de unificado versus Azure AD. '
ms.openlocfilehash: 3427f2401a0e93767f0c563842be323f66d9f21b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036420"
---
# <a name="targetresourcegroup-resource-type"></a>tipo de recurso de targetResourceGroup
Indica o tipo de grupo que foi afetado devido a atividade de auditoria. Inclui valores como os grupos de unificado versus Azure AD. 



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|groupType|String| Os valores possíveis são: `unifiedGroups`, `azureAD`, `unknownFutureValue`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceGroup"
}-->

```json
{
  "groupType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->