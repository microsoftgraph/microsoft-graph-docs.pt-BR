---
title: Tipo de recurso teamCreatedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma equipe criada.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c60ceda4f89832671700ed929bc80b5cb0078edf
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322303"
---
# <a name="teamcreatedeventmessagedetail-resource-type"></a>Tipo de recurso teamCreatedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre uma equipe [criada.](../resources/team.md)
Essa mensagem é gerada quando uma **equipe é** criada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|teamDescription|String|Descrição da **equipe**.|
|teamDisplayName|String|Nome de exibição da **equipe**.|
|teamId|String|Identificador exclusivo da **equipe**.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamCreatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamCreatedEventMessageDetail",
  "teamId": "String",
  "teamDisplayName": "String",
  "teamDescription": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre uma equipe **criada**](/graph/system-messages/#team-created)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
