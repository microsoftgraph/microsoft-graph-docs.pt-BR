---
title: Tipo de recurso teamCreatedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma equipe criada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c90cf71694c2b417de2a364a146334304e00f2dc
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534229"
---
# <a name="teamcreatedeventmessagedetail-resource-type"></a>Tipo de recurso teamCreatedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre uma equipe criada.
Essa mensagem é gerada quando uma equipe é criada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|teamDescription|Cadeia de Caracteres|Descrição da equipe.|
|teamDisplayName|Cadeia de Caracteres|Nome de exibição da equipe.|
|teamId|Cadeia de Caracteres|Identificador exclusivo da equipe.|

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
- [Resposta de exemplo para uma mensagem de evento sobre uma equipe criada](/graph/system-messages/#team-created)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).