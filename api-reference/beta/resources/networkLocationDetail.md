---
title: tipo de recurso networkLocationDetail
description: Indica detalhes associados ao local de rede. .
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3b7e12a87889909737cac9a52fadf64231f7f2a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009605"
---
# <a name="networklocationdetail-resource-type"></a>tipo de recurso networkLocationDetail
Indica detalhes associados ao local de rede.



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|NetworkType|NetworkType|Fornece o tipo da rede. Os valores possíveis são `intranet`: `extranet` `namedNetwork`,, e `trusted`.|
|networknames|Coleção de cadeias de caracteres|Nomes da rede.|


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
