---
title: tipo de recurso chatInfo
description: Contém informações associadas às reuniões do Microsoft Teams.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5801ad39c3e977740825f14da18568a488e77695
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870355"
---
# <a name="chatinfo-resource-type"></a>tipo de recurso chatInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações associadas às reuniões do Microsoft Teams.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição|
|:--------------------|:--------|:-----------|
| messageId           | String  | O identificador exclusivo de uma mensagem em um canal do Microsoft Teams. |
| replyChainMessageId | String  | A ID da mensagem de resposta. |
| threadId            | String  | O identificador exclusivo de um thread no Microsoft Teams. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
