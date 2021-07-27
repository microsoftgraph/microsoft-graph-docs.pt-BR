---
title: Tipo de recurso teamJoiningEnabledEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre a junção de equipe habilitada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 963e53cbb684ed0ab78e0c7eb2e1247f35b5eb2e
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535682"
---
# <a name="teamjoiningenabledeventmessagedetail-resource-type"></a>Tipo de recurso teamJoiningEnabledEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre a junção de equipe habilitada.
Essa mensagem é gerada ao ingressar está habilitada para uma equipe.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|teamId|Cadeia de Caracteres|Identificador exclusivo da equipe.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamJoiningEnabledEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamJoiningEnabledEventMessageDetail",
  "teamId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre a junção de equipe habilitada](/graph/system-messages/#team-joining-enabled)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).