---
title: tipo de recurso de targetResourceServicePrincipal
description: Indica o ServicePrincipalId para o recurso que afetado a atividade de auditoria. Derivado do recurso targetResource.
ms.openlocfilehash: 6d6e19997f4bfead771fc0230207df62dde6c6cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039062"
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