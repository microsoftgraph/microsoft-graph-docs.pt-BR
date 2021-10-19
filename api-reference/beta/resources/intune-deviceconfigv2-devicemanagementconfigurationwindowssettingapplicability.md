---
title: Tipo de recurso deviceManagementConfigurationWindowsSettingApplicability
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a01c2e9721f1748a2e8edcc4b0f008512ec9f8af
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60481080"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a>Tipo de recurso deviceManagementConfigurationWindowsSettingApplicability

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado


Herda [de deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|descrição da configuração Herdada de [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|
|plataforma|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|A configuração da plataforma pode ser aplicada em Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md). Os possíveis valores são: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`.|
|deviceMode|[deviceManagementConfigurationDeviceMode](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|Modo de Dispositivo essa configuração pode ser aplicada em Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md). Os valores possíveis são: `none` e `kiosk`.|
|technologies|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Quais canais de tecnologia essa configuração pode ser implantada por meio de Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md). Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|
|configurationServiceProviderVersion|Cadeia de caracteres|A configuração de versão do CSP faz parte do|
|maximumSupportedVersion|Cadeia de caracteres|Versão máxima com suporte do Windows|
|minimumSupportedVersion|Cadeia de caracteres|Versão mínima com suporte do Windows|
|windowsSkus|[Coleção deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md)|Lista de Windows SKUs que a configuração é aplicável para|
|requiresAzureAd|Booliano|Requisito de configuração do AzureAD|
|requiredAzureAdTrustType|[deviceManagementConfigurationAzureAdTrustType](../resources/intune-deviceconfigv2-devicemanagementconfigurationazureadtrusttype.md)|Tipo de confiança necessário do AzureAD. Os valores possíveis são: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationWindowsSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationWindowsSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String",
  "configurationServiceProviderVersion": "String",
  "maximumSupportedVersion": "String",
  "minimumSupportedVersion": "String",
  "windowsSkus": [
    "String"
  ],
  "requiresAzureAd": true,
  "requiredAzureAdTrustType": "String"
}
```



