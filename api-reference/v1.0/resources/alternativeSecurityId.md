---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno.
ms.localizationpriority: medium
author: spunukol
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9ef21767ee3d38dbba4ad661c0529e2f01a10ba9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036771"
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

