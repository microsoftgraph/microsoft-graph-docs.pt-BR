---
title: tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevicesSummary
description: O resumo de dispositivos de métricas work from anywhere da análise de experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6448bbc89ebe8357fa14a375f82fb73938f6634
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146733"
---
# <a name="userexperienceanalyticsworkfromanywheredevicessummary-resource-type"></a>tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevicesSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O resumo de dispositivos de métricas work from anywhere da análise de experiência do usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|autopilotDevicesSummary|[userExperienceAnalyticsAutopilotDevicesSummary](../resources/intune-devices-userexperienceanalyticsautopilotdevicessummary.md)|O valor do trabalho de qualquer lugar resumo de dispositivos de piloto automático.|
|cloudManagementDevicesSummary|[userExperienceAnalyticsCloudManagementDevicesSummary](../resources/intune-devices-userexperienceanalyticscloudmanagementdevicessummary.md)|A experiência do usuário funciona de qualquer lugar Resumo de dispositivos de gerenciamento de nuvem.|
|windows10DevicesSummary|[userExperienceAnalyticsWindows10DevicesSummary](../resources/intune-devices-userexperienceanalyticswindows10devicessummary.md)|A análise da experiência do usuário funciona em qualquer lugar do resumo de dispositivos Windows 10.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary",
  "autopilotDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
    "devicesNotAutopilotRegistered": 1024,
    "devicesWithoutAutopilotProfileAssigned": 1024
  },
  "cloudManagementDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
    "coManagedDeviceCount": 1024,
    "intuneDeviceCount": 1024,
    "tenantAttachDeviceCount": 1024
  },
  "windows10DevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary",
    "unsupportedOSversionDeviceCount": 1024
  }
}
```




