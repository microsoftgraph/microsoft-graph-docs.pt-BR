---
title: tipo de recurso mediaInfo
description: As informações de mídia usadas em ações para prompts.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8e2f5a0d59f06449d122f4ca2db582afa4da9c39
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965523"
---
# <a name="mediainfo-resource-type"></a>tipo de recurso mediaInfo

Namespace: microsoft.graph

As informações de mídia usadas em ações para prompts.

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    | Descrição                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | String  | Opcional. Usada para identificar exclusivamente o recurso. Se passadas, o URI de prompt será armazenado em cache em relação a este ResourceId como uma chave. |
| URI            | String  | Caminho para o prompt que será reproduzido. O atualmente oferece suporte somente a exemplos de arquivo Wave (. wav), de canal único e 16 bits com uma taxa de amostragem de 16.000 (16 kHz). |


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

