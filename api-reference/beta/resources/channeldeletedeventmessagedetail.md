---
title: Tipo de recurso channelDeletedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre um canal excluído de uma equipe.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0bfbba7d754ec7c40e966315b51122ce8086f356
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535661"
---
# <a name="channeldeletedeventmessagedetail-resource-type"></a>Tipo de recurso channelDeletedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre um canal excluído de uma equipe.
Essa mensagem é gerada quando um canal padrão é excluído de uma equipe.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|channelDisplayName|Cadeia de Caracteres|Nome de exibição do canal.|
|channelId|Cadeia de Caracteres|Identificador exclusivo do canal.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelDeletedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelDeletedEventMessageDetail",
  "channelId": "String",
  "channelDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre um canal excluído de uma equipe](/graph/system-messages/#channel-deleted)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).