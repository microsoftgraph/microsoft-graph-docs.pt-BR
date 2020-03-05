---
title: tipo de recurso chatMessageHostedContent
description: Um conteúdo hospedado em uma mensagem de chat
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a34e09b233a60858e23155f87808e40d080867f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507702"
---
# <a name="chatmessagehostedcontent-resource-type"></a>tipo de recurso chatMessageHostedContent

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o conteúdo hospedado em uma mensagem de chat, como imagens ou trechos de código.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar chatMessageHostedContent](../api/chatmessage-list-chatmessagehostedcontents.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) | Recupere a lista de **chatMessageHostedContent** para uma mensagem. |
| [Obter chatMessageHostedContent](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) | Leia as propriedades e os relacionamentos de um objeto **chatMessageHostedContent** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageHostedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
