---
title: Tipo de recurso tabUpdatedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma guia atualizada.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 020adfcc34a8d2874e021d1b53441093c9f902f7
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322312"
---
# <a name="tabupdatedeventmessagedetail-resource-type"></a>Tipo de recurso tabUpdatedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre uma guia atualizada. Essa mensagem é gerada quando uma guia é atualizada em um [canal](../resources/channel.md) ou [chat](../resources/chat.md).


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|tabId|String|Identificador exclusivo da guia.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.tabUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tabUpdatedEventMessageDetail",
  "tabId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre uma guia atualizada](/graph/system-messages/#tab-updated)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
