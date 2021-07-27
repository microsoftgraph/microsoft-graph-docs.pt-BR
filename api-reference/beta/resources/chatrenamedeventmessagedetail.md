---
title: Tipo de recurso chatRenamedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre um chat renomeado.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a247dd16674a6f7d3173ea5f3f5383d8fd2d68e
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534264"
---
# <a name="chatrenamedeventmessagedetail-resource-type"></a>Tipo de recurso chatRenamedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre um chat renomeado.
Essa mensagem é gerada quando um grupo ou um tópico de chat de reunião é atualizado.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|chatDisplayName|Cadeia de Caracteres|O nome atualizado do chat.|
|chatId|Cadeia de Caracteres|Identificador exclusivo do chat.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatRenamedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatRenamedEventMessageDetail",
  "chatId": "String",
  "chatDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre um chat renomeado](/graph/system-messages/#chat-renamed)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).