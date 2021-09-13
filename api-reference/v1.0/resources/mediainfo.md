---
title: Tipo de recurso mediaInfo
description: As informações de mídia usadas em ações para prompts.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 40bde8c230843156d51b90db64a7e210686886f4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108951"
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

