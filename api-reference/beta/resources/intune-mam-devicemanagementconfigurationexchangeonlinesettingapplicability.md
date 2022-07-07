---
title: Tipo de recurso deviceManagementConfigurationExchangeOnlineSettingApplicability
description: Aplicabilidade para uma configuração Exchange Online configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9bffecb49896ec16d1225fa3e44678429f8f7694
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671442"
---
# <a name="devicemanagementconfigurationexchangeonlinesettingapplicability-resource-type"></a>Tipo de recurso deviceManagementConfigurationExchangeOnlineSettingApplicability

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Aplicabilidade para uma configuração Exchange Online configuração


Herda de [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|descrição da configuração Herdada de [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md)|
|plataforma|[deviceManagementConfigurationPlatforms](../resources/intune-shared-devicemanagementconfigurationplatforms.md)|A configuração da plataforma pode ser aplicada em Herdado de [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md). Os valores possíveis são: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|deviceMode|[deviceManagementConfigurationDeviceMode](../resources/intune-shared-devicemanagementconfigurationdevicemode.md)|Modo de Dispositivo essa configuração pode ser aplicada em Herdado de [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md). Os valores possíveis são: `none` e `kiosk`.|
|Tecnologias|[deviceManagementConfigurationTechnologies](../resources/intune-mam-devicemanagementconfigurationtechnologies.md)|Quais canais de tecnologia essa configuração pode ser implantada por meio de [Herdado de deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md). Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `appleRemoteManagement`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

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




