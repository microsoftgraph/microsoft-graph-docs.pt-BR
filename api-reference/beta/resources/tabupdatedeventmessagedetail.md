---
title: Tipo de recurso tabUpdatedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma guia atualizada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 889645adb05f55d38c0c48bed8c993977401e2dd
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534212"
---
# <a name="tabupdatedeventmessagedetail-resource-type"></a>Tipo de recurso tabUpdatedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre uma guia atualizada. Essa mensagem é gerada quando uma guia é atualizada em um canal ou chat.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|tabId|Cadeia de Caracteres|Identificador exclusivo da guia.|

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