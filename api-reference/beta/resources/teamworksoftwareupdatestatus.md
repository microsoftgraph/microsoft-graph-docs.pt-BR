---
title: tipo de recurso teamworkSoftwareUpdateStatus
description: Representa os detalhes sobre o status de atualização do software para vários componentes, como agente de administração, portal da empresa, firmware, sistema operacional, agente parceiro e cliente Microsoft Teams, em um dispositivo Microsoft Teams habilitado.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a50046c758db26ae1d53507263c65dba7aff7435
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262280"
---
# <a name="teamworksoftwareupdatestatus-resource-type"></a>tipo de recurso teamworkSoftwareUpdateStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre o status de atualização do software para vários componentes, como agente de administração, portal da empresa, firmware, sistema operacional, agente parceiro e cliente Microsoft Teams, em um dispositivo Microsoft Teams [habilitado para Microsoft Teams](../resources/teamworkdevice.md). Indica se uma atualização de software é necessária ou não.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|availableVersion|Cadeia de caracteres|A versão de software disponível a ser atualizada.|
|currentVersion|Cadeia de caracteres|A versão atual do software.|
|softwareFreshness|teamworkSoftwareFreshness|O status de atualização do software. Os valores possíveis são: `unknown`, `latest`, `updateAvailable`, `unknownFutureValue`.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkSoftwareUpdateStatus",
  "availableVersion": "String",
  "currentVersion": "String",
  "softwareFreshness": "String"
}
```

