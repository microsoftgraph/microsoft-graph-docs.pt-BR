---
title: Tipo de recurso teamUnarchivedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma equipe sem hierarquia.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 079a21122b93d8dfa0d9b38579d714aa9b8dea68
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534226"
---
# <a name="teamunarchivedeventmessagedetail-resource-type"></a>Tipo de recurso teamUnarchivedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre uma equipe sem hierarquia.
Essa mensagem é gerada quando uma equipe é desarquivada.


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
- [Resposta de exemplo para uma mensagem de evento sobre uma equipe não ressarquivada](/graph/system-messages/#team-unarchived)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).