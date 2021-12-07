---
title: Tipo de recurso teamsAppInstalledEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre o teamsApp instalado.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8a68e75e98cce394554f165842ecb3b20ed075f9
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322340"
---
# <a name="teamsappinstalledeventmessagedetail-resource-type"></a>Tipo de recurso teamsAppInstalledEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre [o teamsApp](../resources/teamsApp.md) instalado.
Essa mensagem é gerada quando um **teamsApp** é instalado em um [canal](../resources/channel.md), [um chat](../resources/chat.md)ou uma [equipe](../resources/team.md).


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|teamsAppDisplayName|String|Nome de exibição do **teamsApp**.|
|teamsAppId|String|Identificador exclusivo do **teamsApp**.|

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
- [Resposta de exemplo para uma mensagem de evento sobre **teamsApp** instalada](/graph/system-messages/#teams-app-installed)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
