---
title: Tipo de recurso teamArchivedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma equipe arquivada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: eb9334d4cf4d7e8248885c772675c1156405429d
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535686"
---
# <a name="teamarchivedeventmessagedetail-resource-type"></a>Tipo de recurso teamArchivedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre uma equipe arquivada.
Essa mensagem é gerada quando uma equipe é arquivada.


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
- [Resposta de exemplo para uma mensagem de evento sobre uma equipe arquivada](/graph/system-messages/#team-archived)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).