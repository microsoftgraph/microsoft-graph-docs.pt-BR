---
title: tipo de recurso statusBase
description: Descreve o status do evento de Resumo de provisionamento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b63290442f4faddf4bcd9e25c01ab564a7fcc94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520321"
---
# <a name="statusbase-resource-type"></a>tipo de recurso statusBase

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o status do evento de Resumo de provisionamento. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|status|String| Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusBase",
  "baseType": null
}-->

```json
{
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
