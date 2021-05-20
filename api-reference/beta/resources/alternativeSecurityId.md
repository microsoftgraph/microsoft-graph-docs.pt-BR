---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno. Esse tipo complexo será preterido no futuro.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: spunukol
ms.openlocfilehash: 3e696c824e2229ea26cacccee11c93a24d03fa97
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547552"
---
# <a name="alternativesecurityid-resource-type"></a>Tipo de recurso alternativeSecurityId

Namespace: microsoft.graph

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
| identityProvider | cadeia de caracteres     | Apenas para uso interno
| chave              | Edm.Binary | Apenas para uso interno


