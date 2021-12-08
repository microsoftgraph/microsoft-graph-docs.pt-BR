---
title: tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevicesSummary
description: O resumo de dispositivos de métricas work from anywhere da análise de experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f63c579739744f897dd0eaa20e4b53cc75aa966a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335611"
---
# <a name="userexperienceanalyticsworkfromanywheredevicessummary-resource-type"></a>tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevicesSummary

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O resumo de dispositivos de métricas work from anywhere da análise de experiência do usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|autopilotDevicesSummary|[userExperienceAnalyticsAutopilotDevicesSummary](../resources/intune-devices-userexperienceanalyticsautopilotdevicessummary.md)|O valor do trabalho de qualquer lugar resumo de dispositivos de piloto automático.|
|cloudManagementDevicesSummary|[userExperienceAnalyticsCloudManagementDevicesSummary](../resources/intune-devices-userexperienceanalyticscloudmanagementdevicessummary.md)|A experiência do usuário funciona de qualquer lugar Resumo de dispositivos de gerenciamento de nuvem.|
|windows10DevicesSummary|[userExperienceAnalyticsWindows10DevicesSummary](../resources/intune-devices-userexperienceanalyticswindows10devicessummary.md)|A análise de experiência do usuário funciona de qualquer lugar Windows 10 de dispositivos.|
|cloudIdentityDevicesSummary|[userExperienceAnalyticsCloudIdentityDevicesSummary](../resources/intune-devices-userexperienceanalyticscloudidentitydevicessummary.md)|A análise da experiência do usuário funciona de qualquer lugar resumo de dispositivos de Identidade de Nuvem.|
|totalDevices|Int32|A contagem total de dispositivos. Valores válidos -2147483648 para 2147483647|
|coManagedDevices|Int32|Número total de dispositivos co-gerenciados. Valores válidos -2147483648 para 2147483647|
|intuneDevices|Int32|A contagem de dispositivos do intune que não estão no piloto automático registrado. Valores válidos -2147483648 para 2147483647|
|tenantAttachDevices|Int32|Contagem total de dispositivos de anexação de locatários. Valores válidos -2147483648 para 2147483647|
|windows10Devices|Int32|A contagem de dispositivos windows 10. Valores válidos -2147483648 para 2147483647|
|windows10DevicesWithoutTenantAttach|Int32|A contagem de dispositivos windows 10 que são Intune e Comanaged. Valores válidos -2147483648 para 2147483647|
|unsupportedOSversionDevices|Int32|A contagem de Windows 10 que têm versões do sistema operacional sem suporte. Valores válidos -2147483648 para 2147483647|
|devicesWithoutCloudIdentity|Int32|A contagem de dispositivos que não são identidade de nuvem. Valores válidos -2147483648 para 2147483647|
|devicesNotAutopilotRegistered|Int32|A contagem de dispositivos do intune que não estão no piloto automático registrado. Valores válidos -2147483648 para 2147483647|
|devicesWithoutAutopilotProfileAssigned|Int32|A contagem de dispositivos do intune não atribuídos ao perfil de piloto automático. Valores válidos -2147483648 para 2147483647|

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
  },
  "totalDevices": 1024,
  "coManagedDevices": 1024,
  "intuneDevices": 1024,
  "tenantAttachDevices": 1024,
  "windows10Devices": 1024,
  "windows10DevicesWithoutTenantAttach": 1024,
  "unsupportedOSversionDevices": 1024,
  "devicesWithoutCloudIdentity": 1024,
  "devicesNotAutopilotRegistered": 1024,
  "devicesWithoutAutopilotProfileAssigned": 1024
}
```




