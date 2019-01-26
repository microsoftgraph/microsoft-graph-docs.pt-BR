---
title: tipo de recurso de networkLocationDetail
description: Indica detalhes associadas ao local de rede. .
localization_priority: Normal
ms.openlocfilehash: 62bdb23c63beb89b85386e6bea67face097cf1ae
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570936"
---
# <a name="networklocationdetail-resource-type"></a>tipo de recurso de networkLocationDetail
Indica detalhes associadas ao local de rede. .



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|networkType| cadeia de caracteres de enum |Fornece o tipo da rede. Os valores possíveis são `intranet`, `extranet`, `namedNetwork`, e `trusted`.|
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
  "networkTypes": " intranet | extranet | namedNetwork | trusted ",
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
