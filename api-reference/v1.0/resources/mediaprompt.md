---
title: Tipo de recurso mediaPrompt
description: Esse tipo de recurso contém informações sobre o arquivo de áudio a ser tocado e outras configurações adicionais.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b69111bda37ce59305aaf126225f974c25721ceb7ed0ac34af71c1f9bf743438
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141431"
---
# <a name="mediaprompt-resource-type"></a>Tipo de recurso mediaPrompt

Namespace: microsoft.graph

Esse tipo de recurso contém informações sobre o arquivo de áudio a ser tocado e outras configurações adicionais.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo                      | Descrição                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
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
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

