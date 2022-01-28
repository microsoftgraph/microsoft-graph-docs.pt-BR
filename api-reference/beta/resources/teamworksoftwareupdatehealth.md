---
title: tipo de recurso teamworkSoftwareUpdateHealth
description: Representa os detalhes sobre as atualizações de software disponíveis para diferentes componentes, como agente de administração, portal da empresa, firmware, sistema operacional, agente parceiro e cliente Microsoft Teams, em um dispositivo Microsoft Teams habilitado para Microsoft Teams.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8ac1ab4746c83bbcae613c723e1e38ba5f085b4e
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262282"
---
# <a name="teamworksoftwareupdatehealth-resource-type"></a>tipo de recurso teamworkSoftwareUpdateHealth

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre as atualizações de software disponíveis para diferentes componentes, como agente de administração, portal da empresa, firmware, sistema operacional, agente parceiro e cliente Microsoft Teams, em um dispositivo Microsoft Teams [habilitado para Microsoft Teams](../resources/teamworkdevice.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|adminAgentSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|A atualização de software disponível para o agente de administração.|
|companyPortalSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|A atualização de software disponível para o portal da empresa.|
|firmwareSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|A atualização de software disponível para o firmware.|
|operatingSystemSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|A atualização de software disponível para o sistema operacional.|
|partnerAgentSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|A atualização de software disponível para o agente parceiro.|
|teamsClientSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|A atualização de software disponível para o Teams cliente.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkSoftwareUpdateHealth"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkSoftwareUpdateHealth",
  "adminAgentSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "companyPortalSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "firmwareSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "operatingSystemSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "partnerAgentSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "teamsClientSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  }
}
```

