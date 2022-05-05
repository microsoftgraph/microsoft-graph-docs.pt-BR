---
title: Tipo de recurso deviceManagementConfigurationExchangeOnlineSettingApplicability
description: Aplicabilidade para uma configuração Exchange Online configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5608a624f92face6f75898375f41d730ed449649
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205634"
---
# <a name="devicemanagementconfigurationexchangeonlinesettingapplicability-resource-type"></a>Tipo de recurso deviceManagementConfigurationExchangeOnlineSettingApplicability

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Aplicabilidade para uma configuração Exchange Online configuração


Herda de [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|descrição da configuração Herdada de [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|
|plataforma|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|A configuração da plataforma pode ser aplicada em Herdado de [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md). Os valores possíveis são: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|deviceMode|[deviceManagementConfigurationDeviceMode](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|Modo de Dispositivo essa configuração pode ser aplicada em Herdado de [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md). Os valores possíveis são: `none` e `kiosk`.|
|Tecnologias|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Quais canais de tecnologia essa configuração pode ser implantada por meio de [Herdado de deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md). Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `appleRemoteManagement`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationExchangeOnlineSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationExchangeOnlineSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String"
}
```




