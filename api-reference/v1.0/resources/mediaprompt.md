---
title: tipo de recurso mediaPrompt
description: Esse tipo de recurso contém informações sobre o arquivo de áudio a ser reproduzido e outras configurações adicionais.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f981559ce5bac9bb597e49ff1b9d31e48413454b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870994"
---
# <a name="mediaprompt-resource-type"></a>tipo de recurso mediaPrompt

Esse tipo de recurso contém informações sobre o arquivo de áudio a ser reproduzido e outras configurações adicionais.

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
