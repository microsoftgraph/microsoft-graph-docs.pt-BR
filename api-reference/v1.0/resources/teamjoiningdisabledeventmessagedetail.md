---
title: Tipo de recurso teamJoiningDisabledEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre a união de equipe desabilitada.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a7082753265a6be3929f1b697e9e24f9b4e5f95a
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322328"
---
# <a name="teamjoiningdisabledeventmessagedetail-resource-type"></a>Tipo de recurso teamJoiningDisabledEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre [a união](../resources/team.md) de equipe desabilitada.
Essa mensagem é gerada quando a junção é desabilitada para uma **equipe**.


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
  "@odata.type": "microsoft.graph.teamJoiningDisabledEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamJoiningDisabledEventMessageDetail",
  "teamId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre **a junção** de equipe desabilitada](/graph/system-messages/#team-joining-disabled)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
