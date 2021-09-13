---
title: Tipo de recurso chatInfo
description: Informações sobre uma mensagem no Microsoft Teams.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bc548c9f107232368b43aaeb154db2cf5e2cc517
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109427"
---
# <a name="chatinfo-resource-type"></a>Tipo de recurso chatInfo

Namespace: microsoft.graph

Isso contém informações associadas a reuniões Microsoft Teams reuniões.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição|
|:--------------------|:--------|:-----------|
| messageId           | Cadeia de caracteres  | O identificador exclusivo de uma mensagem em um Microsoft Teams canal. |
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

