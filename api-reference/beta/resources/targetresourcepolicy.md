---
title: tipo de recurso de targetResourcePolicy
description: 'Indica a política que foi afetada pela atividade de auditoria. Derivado do recurso targetResource.   '
localization_priority: Normal
ms.openlocfilehash: 355e6ac11741a2aa7aeb780bdac4b7be373092af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813136"
---
# <a name="targetresourcepolicy-resource-type"></a>tipo de recurso de targetResourcePolicy
Indica a política que foi afetada pela atividade de auditoria. Derivado do recurso [targetResource](targetresource.md) .   



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|policyType|Cadeia de caracteres|Indica o nome da política que alterado ou foi direcionados da alteração|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourcePolicy"
}-->

```json
{
  "policyType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourcePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
