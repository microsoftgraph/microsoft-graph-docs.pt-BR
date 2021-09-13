---
title: Tipo de recurso mediaPrompt
description: Esse tipo de recurso contém informações sobre o arquivo de áudio a ser tocado e outras configurações adicionais.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 90630d1ec5d3e4ebc7c30f09f9d5cb66d5daeaaf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108916"
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

