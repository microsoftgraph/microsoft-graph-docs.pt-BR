---
title: Tipo de recurso conditionalAccessPlatforms
description: Plataformas incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 69191885dd3e21aa0ab1f7d4266a33cfe1514e34
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132353"
---
# <a name="conditionalaccessplatforms-resource-type"></a>Tipo de recurso conditionalAccessPlatforms

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Plataformas incluídas e excluídas do escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|includePlatforms|Coleção de cadeias de caracteres| Os possíveis valores são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.|
|excludePlatforms|Coleção de cadeias de caracteres| Os valores possíveis são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPlatforms",
  "baseType": null
}-->

```json
{
  "includePlatforms": ["String"],
  "excludePlatforms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPlatforms resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

