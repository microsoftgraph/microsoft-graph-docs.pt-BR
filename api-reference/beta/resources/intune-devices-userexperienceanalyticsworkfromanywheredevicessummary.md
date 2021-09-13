---
title: tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevicesSummary
description: O resumo de dispositivos de métricas work from anywhere da análise de experiência do usuário.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c3f34ed09d9012f13987aed291ff632f16d064c6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046880"
---
# <a name="userexperienceanalyticsworkfromanywheredevicessummary-resource-type"></a>tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevicesSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O resumo de dispositivos de métricas work from anywhere da análise de experiência do usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|autopilotDevicesSummary|[userExperienceAnalyticsAutopilotDevicesSummary](../resources/intune-devices-userexperienceanalyticsautopilotdevicessummary.md)|O valor do trabalho de qualquer lugar resumo de dispositivos de piloto automático.|
|cloudManagementDevicesSummary|[userExperienceAnalyticsCloudManagementDevicesSummary](../resources/intune-devices-userexperienceanalyticscloudmanagementdevicessummary.md)|A experiência do usuário funciona de qualquer lugar Resumo de dispositivos de gerenciamento de nuvem.|
|windows10DevicesSummary|[userExperienceAnalyticsWindows10DevicesSummary](../resources/intune-devices-userexperienceanalyticswindows10devicessummary.md)|A análise de experiência do usuário funciona de qualquer lugar Windows 10 de dispositivos.|
|cloudIdentityDevicesSummary|[userExperienceAnalyticsCloudIdentityDevicesSummary](../resources/intune-devices-userexperienceanalyticscloudidentitydevicessummary.md)|A análise da experiência do usuário funciona de qualquer lugar resumo de dispositivos de Identidade de Nuvem.|

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
    "devicesWithoutAutopilotProfileAssigned": 1024,
    "totalWindows10DevicesWithoutTenantAttached": 1024
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
  },
  "cloudIdentityDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudIdentityDevicesSummary",
    "deviceWithoutCloudIdentityCount": 1024
  }
}
```



