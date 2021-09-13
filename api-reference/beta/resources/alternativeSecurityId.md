---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno. Esse tipo complexo será preterido no futuro.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: directory-management
author: spunukol
ms.openlocfilehash: 7b646ab42b88a8c74b4bc817593db7770a50b662
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023939"
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


