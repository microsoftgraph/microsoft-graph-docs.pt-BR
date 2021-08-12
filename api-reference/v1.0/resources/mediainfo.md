---
title: Tipo de recurso mediaInfo
description: As informações de mídia usadas em ações para prompts.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8d3a03604a608963c3d5ead22b523f0b8ce3d0979aa34666f4470bad5b61fad1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141424"
---
# <a name="mediainfo-resource-type"></a>Tipo de recurso mediaInfo

Namespace: microsoft.graph

As informações de mídia usadas em ações para prompts.

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    | Descrição                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | Cadeia de caracteres  | Opcional. Usado para identificar exclusivamente o recurso. Se passado, o uri do prompt será armazenado em cache em relação a esse resourceId como uma chave. |
| uri            | Cadeia de caracteres  | Caminho para o prompt que será tocado. Atualmente, só há suporte para formato de arquivo Wave (.wav), amostras de um único canal, de 16 bits com uma taxa de amostragem de 16.000 (16KHz). |


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

