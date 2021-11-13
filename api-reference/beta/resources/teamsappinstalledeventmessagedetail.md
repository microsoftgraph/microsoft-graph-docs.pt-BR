---
title: Tipo de recurso teamsAppInstalledEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre o teamsApp instalado.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3fd14ba502d6caa91442355aee3e590325a95653
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890938"
---
# <a name="teamsappinstalledeventmessagedetail-resource-type"></a>Tipo de recurso teamsAppInstalledEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre uma **instalação do teamsApp.**
Essa mensagem é gerada quando um **teamsApp** é instalado em um canal, um chat ou uma equipe.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|teamsAppDisplayName|Cadeia de Caracteres|Nome de exibição do **teamsApp**.|
|teamsAppId|Cadeia de Caracteres|Identificador exclusivo do **teamsApp**.|

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
