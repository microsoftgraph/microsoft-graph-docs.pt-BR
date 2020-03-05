---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno. Esse tipo complexo será preterido no futuro.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4e3dfae11009000fa89eccb7c0263867fe2a1562
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508328"
---
# <a name="alternativesecurityid-resource-type"></a>Tipo de recurso alternativeSecurityId

Namespace: Microsoft. Graph

Apenas para uso interno. Esse tipo complexo será preterido no futuro.

## <a name="json-representation"></a>Representação JSON

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "type": 12345,
  "identityProvider": "string",
  "key": {"@odata.type": "Edm.Binary"}
}
```

## <a name="properties"></a>Propriedades
| Propriedade         | Tipo       | Descrição
|:-----------------|:-----------|:---------------------
| type             | Int32      | Apenas para uso interno
| identityProvider | string     | Apenas para uso interno
| chave              | Edm.Binary | Apenas para uso interno
