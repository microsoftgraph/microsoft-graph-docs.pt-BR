---
title: Tipo de recurso teamDescriptionUpdatedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma descrição da equipe atualizada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e8694f207801903d3221f0e311a4908bae292302
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535683"
---
# <a name="teamdescriptionupdatedeventmessagedetail-resource-type"></a>Tipo de recurso teamDescriptionUpdatedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre uma descrição da equipe atualizada.
Essa mensagem é gerada quando a descrição de uma equipe é atualizada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|teamDescription|Cadeia de Caracteres|A descrição atualizada para a equipe.|
|teamId|Cadeia de Caracteres|Identificador exclusivo da equipe.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamDescriptionUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamDescriptionUpdatedEventMessageDetail",
  "teamId": "String",
  "teamDescription": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre uma descrição da equipe atualizada](/graph/system-messages/#team-description-updated)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).