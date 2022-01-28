---
title: Tipo de recurso teamworkDeviceSoftwareVersions
description: Representa os detalhes sobre versões de software para um dispositivo Microsoft Teams habilitado.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0605b526e6e3fb3536d1a2fb7c2c14430a8309ed
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262248"
---
# <a name="teamworkdevicesoftwareversions-resource-type"></a>Tipo de recurso teamworkDeviceSoftwareVersions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre versões de software para um dispositivo habilitado para [Microsoft Teams, incluindo](../resources/teamworkdevice.md) firmware, sistema operacional, cliente Microsoft Teams cliente e agente de administração.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|adminAgentSoftwareVersion|Cadeia de caracteres|A versão de software para o agente de administração em execução no dispositivo.|
|firmwareSoftwareVersion|Cadeia de caracteres|A versão de software para o firmware em execução no dispositivo.|
|operatingSystemSoftwareVersion|Cadeia de caracteres|A versão de software do sistema operacional no dispositivo.|
|partnerAgentSoftwareVersion|String|A versão de software para o agente parceiro em execução no dispositivo.|
|teamsClientSoftwareVersion|String|A versão de software para o Teams cliente em execução no dispositivo.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkDeviceSoftwareVersions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceSoftwareVersions",
  "adminAgentSoftwareVersion": "String",
  "firmwareSoftwareVersion": "String",
  "operatingSystemSoftwareVersion": "String",
  "partnerAgentSoftwareVersion": "String",
  "teamsClientSoftwareVersion": "String"
}
```

