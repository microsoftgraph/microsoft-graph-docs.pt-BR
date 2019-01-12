---
title: tipo de recurso de chatInfo
description: Informações sobre uma mensagem em Teams da Microsoft.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 840073d6882d6665be60e7386eaafe3168b70dbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940747"
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
