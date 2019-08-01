---
title: tipo de recurso teamFunSettings
description: Configurações que definem o uso de Giphy, memes e figurinhas na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7605cf55e985791f6723b88485f5a51b2636e026
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033870"
---
# <a name="teamfunsettings-resource-type"></a>tipo de recurso teamFunSettings



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
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
