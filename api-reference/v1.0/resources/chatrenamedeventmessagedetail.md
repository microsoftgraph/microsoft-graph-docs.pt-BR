---
title: Tipo de recurso chatRenamedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre um chat renomeado.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4969a9c165dc957bafd832890597fe58e9629a2d
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322306"
---
# <a name="chatrenamedeventmessagedetail-resource-type"></a>Tipo de recurso chatRenamedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre um [chat renomeado.](../resources/chat.md)
Essa mensagem é gerada quando um grupo ou um tópico **de chat de reunião** é atualizado.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|chatDisplayName|String|O nome atualizado do **chat**.|
|chatId|String|Identificador exclusivo do **chat**.|
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
- [Resposta de exemplo para uma mensagem de evento sobre um **chat renomeado**](/graph/system-messages/#chat-renamed)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
