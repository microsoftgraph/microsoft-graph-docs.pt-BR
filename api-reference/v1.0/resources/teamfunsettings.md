---
title: Tipo de recurso teamFunSettings
description: Configurações que definem o uso de Giphy, memes e figurinhas na equipe.
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 169ecc9ff2e3dfc542a6d055b84234f7a3f98039
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134343"
---
# <a name="teamfunsettings-resource-type"></a>Tipo de recurso teamFunSettings

Namespace: microsoft.graph



Configurações configurar o uso de Giphy, memes e adesivos na [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowGiphy|Boolean|Se definido como true, habilita o uso de Giphy.|
|giphyContentRating|String (enum)|Classificação de conteúdo giphy. Os valores possíveis são: `moderate` e `strict`.|
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

