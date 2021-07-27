---
title: Tipo de recurso teamsAppUpgradedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre teamsApp atualizado.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4bca8bbb7c218333d72cb290e508b352fd977f2d
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535669"
---
# <a name="teamsappupgradedeventmessagedetail-resource-type"></a>Tipo de recurso teamsAppUpgradedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre teamsApp atualizado.
Essa mensagem é gerada quando um teamsApp é atualizado em um canal, um chat ou uma equipe.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|teamsAppDisplayName|Cadeia de Caracteres|Nome de exibição do teamsApp.|
|teamsAppId|Cadeia de Caracteres|Identificador exclusivo do teamsApp.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppUpgradedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppUpgradedEventMessageDetail",
  "teamsAppId": "String",
  "teamsAppDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre o teamsApp atualizado](/graph/system-messages/#teams-app-upgraded)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).