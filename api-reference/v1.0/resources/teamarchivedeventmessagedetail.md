---
title: Tipo de recurso teamArchivedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma equipe arquivada.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3badd933d5ea0c985c0b245a4afc8a6e7b061ff2
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322324"
---
# <a name="teamarchivedeventmessagedetail-resource-type"></a>Tipo de recurso teamArchivedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre uma equipe [arquivada.](../resources/team.md)
Essa mensagem é gerada quando uma **equipe** é arquivada.


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
  "@odata.type": "microsoft.graph.teamArchivedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamArchivedEventMessageDetail",
  "teamId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre uma equipe **arquivada**](/graph/system-messages/#team-archived)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
