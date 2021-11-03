---
title: Tipo de recurso deploymentSettings
description: Determina quando e como o serviço implanta uma atualização.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 0906f401ac414928549602d602317ddc3f5305c5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695710"
---
# <a name="deploymentsettings-resource-type"></a>Tipo de recurso deploymentSettings

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Determina quando e como o serviço implanta uma atualização.

Tipo base [de windowsDeploymentSettings](../resources/windowsupdates-windowsdeploymentsettings.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|monitoring|[microsoft.graph.windowsUpdates.monitoringSettings](../resources/windowsupdates-monitoringsettings.md)|Configurações condições de controle para monitorar e automatizar ações a ser realizadas.|
|lançamento|[microsoft.graph.windowsUpdates.rolloutSettings](../resources/windowsupdates-rolloutsettings.md)|Configurações a forma como o conteúdo é lançado.|
|safeguard|[microsoft.graph.windowsUpdates.safeguardSettings](../resources/windowsupdates-safeguardsettings.md)|Configurações a proteção de controle mantém a oferta de conteúdo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentSettings",
  "rollout": {
    "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
  },
  "monitoring": {
    "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
  },
  "safeguard": {
    "@odata.type": "microsoft.graph.windowsUpdates.safeguardSettings"
  }
}
```

