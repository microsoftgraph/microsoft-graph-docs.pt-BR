---
title: Tipo de recurso chatInfo
description: Informações sobre uma mensagem no Microsoft Teams.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5ae704998bab3015c265d96c188dbcf8eba4729c4df3a1b8a72f3d5076a7f8b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180877"
---
# <a name="chatinfo-resource-type"></a>Tipo de recurso chatInfo

Namespace: microsoft.graph

Isso contém informações associadas a reuniões Microsoft Teams reuniões.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição|
|:--------------------|:--------|:-----------|
| messageId           | String  | O identificador exclusivo de uma mensagem em um Microsoft Teams canal. |
| replyChainMessageId | Cadeia de caracteres  | A ID da mensagem de resposta. |
| threadId            | Cadeia de caracteres  | O identificador exclusivo de um thread no Microsoft Teams. |

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

