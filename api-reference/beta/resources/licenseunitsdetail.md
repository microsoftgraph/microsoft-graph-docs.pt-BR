---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade **prepaidUnits** da entidade subscribedSku é do tipo **licenseUnitsDetail**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: bbff4ac919f5973caff7fbbc30fdc5d7352550b4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807504"
---
# <a name="licenseunitsdetail-resource-type"></a>Tipo de recurso licenseUnitsDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:-------------|:-----|:----------|
|enabled|Int32| O número de unidades que estão habilitadas. |
|suspended|Int32| O número de unidades que estão suspensas. |
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
