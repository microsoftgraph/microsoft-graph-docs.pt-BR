---
title: tipo de recurso mediaInfo
description: As informações de mídia usadas em ações para prompts.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 81fbb1228e8b8821a3a92a6f285a3abc758701ca
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932385"
---
# <a name="mediainfo-resource-type"></a>tipo de recurso mediaInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As informações de mídia usadas em ações para prompts.

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    | Descrição                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | Cadeia de caracteres  | Opcional, usada para identificar exclusivamente o recurso. Se for passado, a URI do prompt será armazenada em cache para esta ResourceId como chave. |
| URI            | String  | Caminho para o prompt a ser reproduzido. Atualmente, somente os exemplos de arquivo Wave (. wav), de canal único e 16 bits com uma taxa de amostragem de 16.000 (16 kHz) só têm suporte. |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
