---
title: Tipo de recurso channelDescriptionUpdatedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma descrição do canal atualizada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6c6d457546b6b9ed757559821defae4e929f9aca
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534231"
---
# <a name="channeldescriptionupdatedeventmessagedetail-resource-type"></a>Tipo de recurso channelDescriptionUpdatedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre uma descrição do canal atualizada.
Essa mensagem é gerada quando a descrição de um canal é atualizada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|channelDescription|Cadeia de Caracteres|A descrição atualizada do canal.|
|channelId|Cadeia de Caracteres|Identificador exclusivo do canal.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelDescriptionUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelDescriptionUpdatedEventMessageDetail",
  "channelId": "String",
  "channelDescription": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre uma descrição de canal atualizada](/graph/system-messages/#channel-description-updated)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).