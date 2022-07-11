---
title: Tipo de recurso deviceManagementConfigurationWindowsSettingApplicability
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e82561136e1706b5b4fd059dee0d33a15d13836e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671539"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a>Tipo de recurso deviceManagementConfigurationWindowsSettingApplicability

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado


Herda de [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|descrição da configuração Herdada de [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md)|
|plataforma|[deviceManagementConfigurationPlatforms](../resources/intune-shared-devicemanagementconfigurationplatforms.md)|A configuração da plataforma pode ser aplicada em Herdado de [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md). Os valores possíveis são: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|deviceMode|[deviceManagementConfigurationDeviceMode](../resources/intune-shared-devicemanagementconfigurationdevicemode.md)|Modo de Dispositivo essa configuração pode ser aplicada em Herdado de [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md). Os valores possíveis são: `none` e `kiosk`.|
|Tecnologias|[deviceManagementConfigurationTechnologies](../resources/intune-mam-devicemanagementconfigurationtechnologies.md)|Quais canais de tecnologia essa configuração pode ser implantada por meio de [Herdado de deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md). Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `appleRemoteManagement`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|
|configurationServiceProviderVersion|Cadeia de Caracteres|A versão da configuração do CSP faz parte do|
|maximumSupportedVersion|Cadeia de caracteres|Versão máxima com suporte do Windows|
|minimumSupportedVersion|Cadeia de Caracteres|Versão mínima com suporte do Windows|
|windowsSkus|[Coleção deviceManagementConfigurationWindowsSkus](../resources/intune-shared-devicemanagementconfigurationwindowsskus.md)|Lista de SKUs do Windows para as qual a configuração é aplicável|
|requiresAzureAd|Booliano|Requisito de configuração do AzureAD|
|requiredAzureAdTrustType|[deviceManagementConfigurationAzureAdTrustType](../resources/intune-shared-devicemanagementconfigurationazureadtrusttype.md)|Tipo de confiança necessário do AzureAD. Os valores possíveis são: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.|

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




