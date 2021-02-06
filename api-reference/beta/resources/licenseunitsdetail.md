---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade **prepaidUnits** da entidade subscribedSku é do tipo **licenseUnitsDetail**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: krbain
ms.openlocfilehash: 3d4925c2acea0216e16283eaa8f779cb556e0857
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132430"
---
# <a name="licenseunitsdetail-resource-type"></a>Tipo de recurso licenseUnitsDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:-------------|:-----|:----------|
|enabled|Int32| O número de unidades habilitadas. |
|suspended|Int32| O número de unidades suspensas. |
|warning|Int32| O número de unidades que estão no status de aviso. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


