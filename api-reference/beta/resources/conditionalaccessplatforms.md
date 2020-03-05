---
title: tipo de recurso conditionalAccessPlatforms
description: Plataformas incluídas e excluídas do escopo da política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2612b352f512d1177bc9137603b6ecda1ad96f66
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507531"
---
# <a name="conditionalaccessplatforms-resource-type"></a>tipo de recurso conditionalAccessPlatforms

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Plataformas incluídas e excluídas do escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|includePlatforms|String collection| Os possíveis valores são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.|
|excludePlatforms|String collection| Os valores possíveis são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.|

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