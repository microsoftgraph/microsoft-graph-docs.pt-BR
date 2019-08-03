---
title: tipo de recurso educationMakeCodeResource
description: Um recurso MakeCode
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e983f217af71b6e27f750599ee2f8db295da5fec
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173367"
---
# <a name="educationmakecoderesource-resource-type"></a>tipo de recurso educationMakeCodeResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um recurso representando um projeto [MakeCode](https://www.microsoft.com/en-us/makecode) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|mkcd|String|ID do projeto MakeCode|
|url|Cadeia de caracteres|Host para o tipo de recurso MakeCode (por exemplo,, MICROBIT)|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationMakeCodeResource",
  "baseType": "microsoft.graph.educationResource"
}-->

```json
{
  "mkcd": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationMakeCodeResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->