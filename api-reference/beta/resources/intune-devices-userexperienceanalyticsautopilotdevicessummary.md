---
title: tipo de recurso userExperienceAnalyticsAutopilotDevicesSummary
description: O resumo de análise de experiência do usuário de Dispositivos que não estão prontos para o windows autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 27faa3cf52ba5b0118137b1d64c63552d9e4f127
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159336"
---
# <a name="userexperienceanalyticsautopilotdevicessummary-resource-type"></a>tipo de recurso userExperienceAnalyticsAutopilotDevicesSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O resumo de análise de experiência do usuário de Dispositivos que não estão prontos para o windows autopilot.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|devicesNotAutopilotRegistered|Int32|A contagem de dispositivos do intune que não estão no piloto automático registrado.|
|devicesWithoutAutopilotProfileAssigned|Int32|A contagem de dispositivos do intune não atribuídos ao perfil de piloto automático.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
  "devicesNotAutopilotRegistered": 1024,
  "devicesWithoutAutopilotProfileAssigned": 1024
}
```




