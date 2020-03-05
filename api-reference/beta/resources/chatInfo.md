---
title: tipo de recurso chatInfo
description: Contém informações associadas às reuniões do Microsoft Teams.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8602301af0de458f07ab5a9c0af00ec8578c3a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507730"
---
# <a name="chatinfo-resource-type"></a>tipo de recurso chatInfo

Namespace: Microsoft. Graph

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
