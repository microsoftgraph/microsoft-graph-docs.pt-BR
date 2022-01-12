---
title: Tipo de recurso windowsDeploymentSettings
description: Configurações controlar quando e como o serviço implanta uma Windows 10 atualização.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 16aa8592dc03dda799ffbddf838520ca0f159192
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861369"
---
# <a name="windowsdeploymentsettings-resource-type"></a>Tipo de recurso windowsDeploymentSettings

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações controlar quando e como o serviço implanta uma Windows 10 atualização.

Herda de [deploymentSettings](../resources/windowsupdates-deploymentsettings.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|monitoring|[microsoft.graph.windowsUpdates.monitoringSettings](../resources/windowsupdates-monitoringsettings.md)|Configurações condições de controle para monitorar e automatizar ações a ser realizadas. Herdado [de deploymentSettings](../resources/windowsupdates-deploymentsettings.md).|
|lançamento|[microsoft.graph.windowsUpdates.rolloutSettings](../resources/windowsupdates-rolloutsettings.md)|Configurações a forma como o conteúdo é lançado. Herdado [de deploymentSettings](../resources/windowsupdates-deploymentsettings.md).|
|userExperience|[microsoft.graph.windowsUpdates.userExperienceSettings](../resources/windowsupdates-userexperiencesettings.md)|Configurações a experiência de atualização do usuário em um dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windowsDeploymentSettings",
  "rollout": {
    "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
  },
  "monitoring": {
    "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
  },
  "userExperience": {
    "@odata.type": "microsoft.graph.windowsUpdates.userExperienceSettings"
  }
}
```

