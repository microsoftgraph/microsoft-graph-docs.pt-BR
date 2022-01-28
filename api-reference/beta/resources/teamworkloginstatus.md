---
title: Tipo de recurso teamworkLoginStatus
description: Representa Microsoft Teams, Skype for Business e Exchange de entrada para um dispositivo Microsoft Teams habilitado.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 460b9bfb341f7b8a564347f0ab4f64d824120d09
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262355"
---
# <a name="teamworkloginstatus-resource-type"></a>Tipo de recurso teamworkLoginStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa Microsoft Teams, Skype for Business e Exchange de entrada para um dispositivo Microsoft Teams [habilitado](../resources/teamworkdevice.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|exchangeConnection|[teamworkConnection](../resources/teamworkconnection.md)|Informações sobre a Exchange conexão.|
|skypeConnection|[teamworkConnection](../resources/teamworkconnection.md)|Informações sobre a conexão Skype for Business.|
|teamsConnection|[teamworkConnection](../resources/teamworkconnection.md)|Informações sobre a Teams conexão.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkLoginStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkLoginStatus",
  "exchangeConnection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  },
  "teamsConnection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  },
  "skypeConnection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  }
}
```

