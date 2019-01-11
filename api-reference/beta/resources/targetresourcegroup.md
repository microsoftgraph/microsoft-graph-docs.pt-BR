---
title: tipo de recurso de targetResourceGroup
description: 'Indica o tipo de grupo que foi afetado devido a atividade de auditoria. Inclui valores como os grupos de unificado versus Azure AD. '
localization_priority: Normal
ms.openlocfilehash: 2cc7e0adb1a93394b64375d05dfb6a6e349bac55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851181"
---
# <a name="targetresourcegroup-resource-type"></a>tipo de recurso de targetResourceGroup
Indica o tipo de grupo que foi afetado devido a atividade de auditoria. Inclui valores como os grupos de unificado versus Azure AD. 



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|groupType|Cadeia de caracteres| Os valores possíveis são: `unifiedGroups`, `azureAD`, `unknownFutureValue`.|

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
