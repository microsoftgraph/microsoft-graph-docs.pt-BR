---
title: Tipo de recurso teamworkDisplayConfiguration
description: Representa os detalhes sobre a configuração de exibição de um dispositivo Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 88de0c02af3012b1fff55f4ef1cb0f58773c4f7b
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262244"
---
# <a name="teamworkdisplayconfiguration-resource-type"></a>Tipo de recurso teamworkDisplayConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre a configuração de exibição de um dispositivo Microsoft Teams habilitado [para Microsoft Teams.](../resources/teamworkdevice.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|configuredDisplays|[coleção teamworkConfiguredPeripheral](../resources/teamworkconfiguredperipheral.md)|A lista de exibições configuradas. Aplicável somente para Salas do Microsoft Teams dispositivos.|
|displayCount|Int32|Número total de exibições conectadas, incluindo a tela inbuilt. Aplicável somente para Salas do Teams dispositivos.|
|inBuiltDisplayScreenConfiguration|[teamworkDisplayScreenConfiguration](../resources/teamworkdisplayscreenconfiguration.md)|Configuração para a exibição inbuilt. Não aplicável para Salas do Teams dispositivos.|
|isContentDuplicationAllowed|Booliano|`True` se a duplicação de conteúdo for permitida. Aplicável somente para Salas do Teams dispositivos.|
|isDualDisplayModeEnabled|Booliano|`True` se o modo de exibição dual estiver habilitado. Se **isDualDisplayModeEnabled** `true`for , o conteúdo será exibido em ambas as telas de sala em vez de apenas uma tela, quando ele for compartilhado por meio do módulo de ingestão HDMI no dispositivo Salas do Microsoft Teams. Aplicável somente para Salas do Teams dispositivos.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkDisplayConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDisplayConfiguration",
  "configuredDisplays": [
    {
      "@odata.type": "microsoft.graph.teamworkConfiguredPeripheral"
    }
  ],
  "displayCount": "Integer",
  "inBuiltDisplayScreenConfiguration": {
    "@odata.type": "microsoft.graph.teamworkDisplayScreenConfiguration"
  },
  "isContentDuplicationAllowed": "Boolean",
  "isDualDisplayModeEnabled": "Boolean"
}
```

