---
title: tipo de recurso do minhas informações
description: tipo de recurso do minhas informações
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: daca733578e5415fc777bc01a8ef1272cfdcc681
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228877"
---
# <a name="serviceinformation-resource-type"></a>tipo de recurso do minhas informações

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dados descritivos básicos sobre os serviços de nuvem que um usuário optou por consultar de sua conta.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|nome          | Cadeia de caracteres      | O nome do serviço de nuvem (por exemplo, Twitter, Instagram). |
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
