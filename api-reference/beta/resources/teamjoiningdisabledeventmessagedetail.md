---
title: Tipo de recurso teamJoiningDisabledEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre a união de equipe desabilitada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a509b23ef7239a9f8d75cc7895b2c4f7a53b50d4
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534228"
---
# <a name="teamjoiningdisabledeventmessagedetail-resource-type"></a>Tipo de recurso teamJoiningDisabledEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre a união de equipe desabilitada.
Essa mensagem é gerada quando a junção é desabilitada para uma equipe.


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
- [Resposta de exemplo para uma mensagem de evento sobre a junção de equipe desabilitada](/graph/system-messages/#team-joining-disabled)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).