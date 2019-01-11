---
title: tipo de recurso de targetResourceServicePrincipal
description: Indica o ServicePrincipalId para o recurso que afetado a atividade de auditoria. Derivado do recurso targetResource.
localization_priority: Normal
ms.openlocfilehash: 37bd63851ca9169afb669c710ef4cb2c150ea615
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839596"
---
# <a name="targetresourceserviceprincipal-resource-type"></a>tipo de recurso de targetResourceServicePrincipal
Indica o ServicePrincipalId para o recurso que afetado a atividade de auditoria. Derivado do recurso [targetResource](targetresource.md) .



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appId|Cadeia de caracteres|Indica a Id exclusiva do aplicativo. Se refere à Id de aplicativo para um aplicativo específico.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceServicePrincipal"
}-->

```json
{
  "appId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
