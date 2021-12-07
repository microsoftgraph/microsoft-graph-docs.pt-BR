---
title: Tipo de recurso teamRenamedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma equipe renomeada.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c1569be468116d539d0144519d0225975abf004b
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322295"
---
# <a name="teamrenamedeventmessagedetail-resource-type"></a>Tipo de recurso teamRenamedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre uma equipe [renomeada.](../resources/team.md)
Essa mensagem é gerada quando o **nome de uma** equipe é atualizado.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|teamDisplayName|String|O nome atualizado da **equipe**.|
|teamId|String|Identificador exclusivo da **equipe**.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamRenamedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamRenamedEventMessageDetail",
  "teamId": "String",
  "teamDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre uma equipe **renomeada**](/graph/system-messages/#team-renamed)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
