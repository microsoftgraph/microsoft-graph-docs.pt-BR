---
title: Tipo de recurso messageUnpinnedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma mensagem de chat desafixada.
author: sumanac
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 28cdd335bf2d11d934782f5f94d359865b5b5b50
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118671"
---
# <a name="messageunpinnedeventmessagedetail-resource-type"></a>Tipo de recurso messageUnpinnedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre um [chatMessage desafixado](../resources/chatmessage.md). Essa mensagem é gerada quando uma mensagem de chat é desafixada.

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
  "@odata.type": "microsoft.graph.messageUnpinnedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.messageUnpinnedEventMessageDetail",
  "eventDateTime": "String (timestamp)",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Exemplo de resposta para uma mensagem de evento sobre uma mensagem de chat desafixada](/graph/system-messages/#message-unpinned)
- Para obter mais informações sobre outros tipos de eventos, consulte [Mensagens do sistema](/graph/system-messages).
