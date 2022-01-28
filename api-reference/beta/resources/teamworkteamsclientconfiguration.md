---
title: Tipo de recurso teamworkTeamsClientConfiguration
description: Representa detalhes de configuração para o cliente Microsoft Teams em execução em um Salas do Microsoft Teams dispositivo.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 46c1ac98c9992df65441dd3b92e12f81ae8804b0
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262367"
---
# <a name="teamworkteamsclientconfiguration-resource-type"></a>Tipo de recurso teamworkTeamsClientConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes de configuração para o cliente Microsoft Teams em execução em um Salas do Microsoft Teams [dispositivo](../resources/teamworkdevice.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accountConfiguration|[teamworkAccountConfiguration](../resources/teamworkaccountconfiguration.md)|A configuração da conta Microsoft Teams cliente para um dispositivo.|
|featuresConfiguration|[teamworkFeaturesConfiguration](../resources/teamworkfeaturesconfiguration.md)|A configuração de Microsoft Teams de cliente para um dispositivo.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkTeamsClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTeamsClientConfiguration",
  "accountConfiguration": {
    "@odata.type": "microsoft.graph.teamworkAccountConfiguration"
  },
  "featuresConfiguration": {
    "@odata.type": "microsoft.graph.teamworkFeaturesConfiguration"
  }
}
```

