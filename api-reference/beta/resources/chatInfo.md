---
title: tipo de recurso de chatInfo
description: Informações sobre uma mensagem em Teams da Microsoft.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: c2cc0dd288abdab7852017600c4c55b9a40b0aa7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852938"
---
# <a name="chatinfo-resource-type"></a>tipo de recurso de chatInfo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Informações sobre uma mensagem em Teams da Microsoft.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição|
|:--------------------|:--------|:-----------|
| messageId           | Cadeia de caracteres  | O identificador exclusivo para uma mensagem em um canal de Teams da Microsoft. |
| replyChainMessageId | Cadeia de caracteres  | A ID da mensagem de resposta. |
| threadId            | Cadeia de caracteres  | O identificador exclusivo de um segmento no Microsoft Teams. |

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
<!-- {
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
