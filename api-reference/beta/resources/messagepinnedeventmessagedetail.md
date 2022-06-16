---
title: Tipo de recurso messagePinnedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma mensagem de chat fixada.
author: sumanac
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: acec5aaf817549c6ac4913b2aced914ee6a497d2
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118667"
---
# <a name="messagepinnedeventmessagedetail-resource-type"></a>Tipo de recurso messagePinnedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre um [chatMessage fixado](../resources/chatmessage.md). Essa mensagem é gerada quando uma mensagem de chat é fixada.

Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|eventDateTime|DateTimeOffset|Data e hora em que o evento ocorreu.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.messagePinnedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.messagePinnedEventMessageDetail",
  "eventDateTime": "String (timestamp)",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Exemplo de resposta para uma mensagem de evento sobre uma mensagem de chat fixada](/graph/system-messages/#message-pinned)
- Para obter mais informações sobre outros tipos de eventos, consulte [Mensagens do sistema](/graph/system-messages).
