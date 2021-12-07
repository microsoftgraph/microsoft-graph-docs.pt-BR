---
title: Tipo de recurso channelDeletedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre um canal excluído de uma equipe.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99a009ac2fd967a8ebcc3a7a688f34e0f84cdfde
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322317"
---
# <a name="channeldeletedeventmessagedetail-resource-type"></a>Tipo de recurso channelDeletedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre um [canal](../resources/channel.md) excluído de uma [equipe](../resources/team.md).
Essa mensagem é gerada quando um canal **padrão** é excluído de uma **equipe**.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|channelDisplayName|String|Nome de exibição do **canal**.|
|channelId|String|Identificador exclusivo do **canal**.|
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
- [Resposta de exemplo para uma mensagem de evento sobre **um canal** excluído de uma **equipe**](/graph/system-messages/#channel-deleted)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
