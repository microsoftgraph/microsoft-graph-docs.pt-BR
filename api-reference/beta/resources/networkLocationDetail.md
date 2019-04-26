---
title: tipo de recurso networkLocationDetail
description: Indica detalhes associados ao local de rede. .
localization_priority: Normal
ms.openlocfilehash: c4a5323099258d9670b970b1bb85bd0d01f3cf8d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342174"
---
# <a name="networklocationdetail-resource-type"></a>tipo de recurso networkLocationDetail
Indica detalhes associados ao local de rede.



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|NetworkType|NetworkType|Fornece o tipo da rede. Os valores possíveis são `intranet`: `extranet` `namedNetwork`,, e `trusted`.|
|networknames|Coleção String|Nomes da rede.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail"
}-->

```json
{
  "networkType": "string",
  "networkNames": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
