---
title: Tipo de recurso teamsAppInstalledEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre o teamsApp instalado.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 04ed2f02c64d5339f0343445614ef7cf7a069f2a
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535671"
---
# <a name="teamsappinstalledeventmessagedetail-resource-type"></a>Tipo de recurso teamsAppInstalledEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre o teamsApp instalado.
Essa mensagem é gerada quando um teamsApp é instalado em um canal, um chat ou uma equipe.


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
  "@odata.type": "microsoft.graph.teamsAppInstalledEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppInstalledEventMessageDetail",
  "teamsAppId": "String",
  "teamsAppDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre teamsApp instalada](/graph/system-messages/#teams-app-installed)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).