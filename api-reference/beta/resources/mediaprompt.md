---
title: tipo de recurso de mediaPrompt
description: O tipo de mediaPrompt.
ms.openlocfilehash: 1a782d391110d35b07b551e44ebd3b931dbcadba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039242"
---
# <a name="mediaprompt-resource-type"></a>tipo de recurso de mediaPrompt

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O tipo de mediaPrompt.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo                      | Descrição                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| loop        | Int32                     | A contagem de loop. o valor 0 indica para executar um loop indefinidamente. O valor padrão é `1`. |
| mediaInfo   | [mediaInfo](mediainfo.md) | As informações de mídia                                                           |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "loop": 1024,
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a>Exemplo

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "mediaInfo": {
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  },
  "loop": 5
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
