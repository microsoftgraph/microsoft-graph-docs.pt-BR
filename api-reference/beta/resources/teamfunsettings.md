---
title: tipo de recurso de teamFunSettings
description: Configurações para configurar o uso de Giphy, memes e adesivos na equipe de.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: b4c30afb6d0c10e8f011b779cf257a1627ff7b48
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949777"
---
# <a name="teamfunsettings-resource-type"></a>tipo de recurso de teamFunSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Configurações para configurar o uso de Giphy, adesivos e memes em [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowGiphy|Booliano|Se definido como true, permite que o uso de Giphy.|
|giphyContentRating|Cadeia de caracteres (enum)|Classificação de conteúdo Giphy. Os valores possíveis são: `moderate` e `strict`.|
|allowStickersAndMemes|Booliano|Se definido como true, permite que os usuários incluem adesivos e memes.|
|allowCustomMemes|Booliano|Se definido como true, permite que os usuários incluem memes personalizado.|

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
