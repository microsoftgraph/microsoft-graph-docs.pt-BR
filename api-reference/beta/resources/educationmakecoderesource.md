---
title: tipo de recurso educationMakeCodeResource
description: Um recurso MakeCode
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 708efc4e72abeba9ff0acfe6e4768c61518e1a6b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501707"
---
# <a name="educationmakecoderesource-resource-type"></a>tipo de recurso educationMakeCodeResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um recurso representando um projeto [MakeCode](https://www.microsoft.com/en-us/makecode) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|projectId|String|ID do projeto MakeCode|
|hostWebUrl|String|Host para o tipo de recurso MakeCode (por exemplo,, MICROBIT)|

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
  "projectId": "String",
  "hostWebUrl": "String"
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