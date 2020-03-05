---
title: tipo de recurso do minhas informações
description: tipo de recurso do minhas informações
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7b121a1bd3369eebd752651fa412510daf943b76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520784"
---
# <a name="serviceinformation-resource-type"></a>tipo de recurso do minhas informações

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dados descritivos básicos sobre os serviços de nuvem que um usuário optou por consultar de sua conta.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                            |
|:-------------|:------------|:-------------------------------------------------------|
|nome          | Cadeia de caracteres      | O nome do serviço de nuvem (por exemplo, Twitter, Instagram). |
|webUrl        | String      | Contém a URL para o serviço que está sendo referenciado.     |

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
