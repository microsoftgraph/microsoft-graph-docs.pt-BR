---
title: tipo de recurso de networkLocationDetail
description: Indica detalhes associadas ao local de rede. .
ms.openlocfilehash: 5dd1410318d380a1b943de6a7dbb0d739172cc76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037625"
---
# <a name="networklocationdetail-resource-type"></a>tipo de recurso de networkLocationDetail
Indica detalhes associadas ao local de rede. .



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|networkType|String|Fornece o tipo da rede. Os valores possíveis são `intranet`, `extranet`, `namedNetwork`, e `trusted`.|
|networkName|String|Nome da rede.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": "namedNetork",
  "networkName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->