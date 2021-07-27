---
title: Tipo de recurso teamsAppRemovedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre teamsApp removida.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 24d080e77d679e0e12970be2b78ea3af7b4d6668
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535670"
---
# <a name="teamsappremovedeventmessagedetail-resource-type"></a>Tipo de recurso teamsAppRemovedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre teamsApp removida.
Essa mensagem é gerada quando um teamsApp é removido de um canal, de um chat ou de uma equipe.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|teamsAppDisplayName|Cadeia de Caracteres|Nome de exibição do teamApp.|
|teamsAppId|Cadeia de Caracteres|Identificador exclusivo do teamsApp.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppRemovedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppRemovedEventMessageDetail",
  "teamsAppId": "String",
  "teamsAppDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre teamsApp removida](/graph/system-messages/#teams-app-removed)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).