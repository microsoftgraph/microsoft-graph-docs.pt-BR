---
title: tipo de recurso teamFunSettings
description: Configurações que definem o uso de Giphy, memes e figurinhas na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a58879c73e86dac6326576739c6a959a7e1efa78
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046647"
---
# <a name="teamfunsettings-resource-type"></a>tipo de recurso teamFunSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações para configurar o uso de Giphy, memes e selos na [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowGiphy|Booliano|Se definido como true, habilita o uso do Giphy.|
|giphyContentRating|Cadeia de caracteres (enum)|Classificação de conteúdo do Giphy. Os valores possíveis são: `moderate` e `strict`.|
|allowStickersAndMemes|Booliano|Se definido como true, permite que os usuários incluam adesivos e memes.|
|allowCustomMemes|Booliano|Se definido como true, permite que os usuários incluam memes personalizados.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


