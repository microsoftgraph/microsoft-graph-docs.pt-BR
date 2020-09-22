---
title: tipo de recurso do minhas informações
description: tipo de recurso do minhas informações
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 39382b0fb17795bde26b4e54f629b2e4281f81db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070438"
---
# <a name="serviceinformation-resource-type"></a>tipo de recurso do minhas informações

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dados descritivos básicos sobre os serviços de nuvem que um usuário optou por consultar de sua conta.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|name          | Cadeia de caracteres      | O nome do serviço de nuvem (por exemplo, Twitter, Instagram). |
|webUrl        | String      | Contém a URL para o serviço que está sendo referenciado.               |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.serviceInformation",
  "baseType": null
}-->

```json
{
  "name": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


