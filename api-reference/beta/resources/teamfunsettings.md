---
title: tipo de recurso de teamFunSettings
description: Configurações para configurar o uso de Giphy, memes e adesivos na equipe de.
ms.openlocfilehash: e8cf62b88a3afa3e5caf6b9425312d7a26af4d20
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033552"
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
