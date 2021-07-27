---
title: Tipo de recurso channelRenamedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre um canal renomeado.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7ffe2ae896a0f313f08d5af32753c4806831575c
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535660"
---
# <a name="channelrenamedeventmessagedetail-resource-type"></a>Tipo de recurso channelRenamedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre um canal renomeado.
Essa mensagem é gerada quando o nome de um canal é atualizado.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|channelDisplayName|Cadeia de Caracteres|O nome atualizado do canal.|
|channelId|Cadeia de Caracteres|Identificador exclusivo do canal.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelRenamedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelRenamedEventMessageDetail",
  "channelId": "String",
  "channelDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre um canal renomeado](/graph/system-messages/#channel-renamed)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
