---
title: Tipo de recurso userExperienceAnalyticsBatteryHealthDeviceAppImpact
description: A entidade de impacto do aplicativo de dispositivo de saúde da bateria de análise de experiência do usuário contém informações relacionadas ao uso da bateria em um nível de aplicativo para um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6e1e9dafdc831528ff9d05115f86a68b1df328d4
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348065"
---
# <a name="userexperienceanalyticsbatteryhealthdeviceappimpact-resource-type"></a>Tipo de recurso userExperienceAnalyticsBatteryHealthDeviceAppImpact

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de impacto do aplicativo de dispositivo de saúde da bateria de análise de experiência do usuário contém informações relacionadas ao uso da bateria em um nível de aplicativo para um determinado dispositivo.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsBatteryHealthDeviceAppImpacts](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-list.md)|[coleção userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsBatteryHealthDeviceAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|
|[Obter userExperienceAnalyticsBatteryHealthDeviceAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-get.md)|[userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsBatteryHealthDeviceAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|
|[Criar userExperienceAnalyticsBatteryHealthDeviceAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-create.md)|[userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|Crie um novo [objeto userExperienceAnalyticsBatteryHealthDeviceAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|
|[Excluir userExperienceAnalyticsBatteryHealthDeviceAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-delete.md)|Nenhum|Exclui um [usuárioExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md).|
|[Atualizar userExperienceAnalyticsBatteryHealthDeviceAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-update.md)|[userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsBatteryHealthDeviceAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de impacto do aplicativo do dispositivo de bateria de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|O identificador exclusivo do dispositivo, id do dispositivo Intune DeviceID ou SCCM.|
|appName|Cadeia de caracteres|Nome do aplicativo. Por exemplo: oltk.exe|
|appDisplayName|String|Nome de exibição amigável para o aplicativo. Por exemplo: Outlook|
|appPublisher|String|Editor de aplicativos. Por exemplo: Microsoft Corporation|
|isForegroundApp|Booliano|true se o usuário teve interação ativa com o aplicativo.|
|batteryUsagePercentage|Duplo|A porcentagem da energia total da bateria usada por esse aplicativo quando o dispositivo não foi conectado à energia ac, por mais de 14 dias. Unidade em porcentagem. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceAppImpact"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceAppImpact",
  "id": "String (identifier)",
  "deviceId": "String",
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "isForegroundApp": true,
  "batteryUsagePercentage": "4.2"
}
```




