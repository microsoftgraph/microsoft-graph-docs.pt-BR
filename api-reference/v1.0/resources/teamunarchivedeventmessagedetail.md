---
title: Tipo de recurso teamUnarchivedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma equipe sem hierarquia.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: adb8e6c0d8ebfc83f973c730fd0a36454df5d8ef
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322294"
---
# <a name="teamunarchivedeventmessagedetail-resource-type"></a>Tipo de recurso teamUnarchivedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre uma equipe sem [hierarquia.](../resources/team.md)
Essa mensagem é gerada quando uma **equipe** é desarquivada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|teamId|String|Identificador exclusivo da **equipe**.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamUnarchivedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamUnarchivedEventMessageDetail",
  "teamId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre uma equipe não **ressarquivada**](/graph/system-messages/#team-unarchived)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
