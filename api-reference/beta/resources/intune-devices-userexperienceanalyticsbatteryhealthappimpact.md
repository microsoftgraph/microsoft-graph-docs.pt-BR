---
title: Tipo de recurso userExperienceAnalyticsBatteryHealthAppImpact
description: A entidade de impacto do aplicativo de saúde da bateria de análise de experiência do usuário contém informações relacionadas ao uso da bateria em um nível de aplicativo para o locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ef986108396bd1dbdb013be810aea01ebd1e6627
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342409"
---
# <a name="userexperienceanalyticsbatteryhealthappimpact-resource-type"></a>Tipo de recurso userExperienceAnalyticsBatteryHealthAppImpact

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de impacto do aplicativo de saúde da bateria de análise de experiência do usuário contém informações relacionadas ao uso da bateria em um nível de aplicativo para o locatário.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsBatteryHealthAppImpacts](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-list.md)|[Coleção userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsBatteryHealthAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|
|[Obter userExperienceAnalyticsBatteryHealthAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-get.md)|[userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsBatteryHealthAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|
|[Criar userExperienceAnalyticsBatteryHealthAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-create.md)|[userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|Crie um novo [objeto userExperienceAnalyticsBatteryHealthAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|
|[Excluir userExperienceAnalyticsBatteryHealthAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md).|
|[Atualizar userExperienceAnalyticsBatteryHealthAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-update.md)|[userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsBatteryHealthAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de impacto do aplicativo de bateria de análise de experiência do usuário.|
|activeDevices|Int32|Número de dispositivos ativos para usar esse aplicativo em um período de 14 dias. Valores válidos -2147483648 para 2147483647|
|appName|Cadeia de caracteres|Nome do aplicativo. Por exemplo: oltk.exe|
|appDisplayName|String|Nome de exibição amigável para o aplicativo. Por exemplo: Outlook|
|appPublisher|String|Editor de aplicativos. Por exemplo: Microsoft Corporation|
|isForegroundApp|Booliano|true se o usuário teve interação ativa com o aplicativo.|
|batteryUsagePercentage|Duplo|A porcentagem da energia total da bateria usada por esse aplicativo quando o dispositivo não estava conectado à energia ac, mais de 14 dias computado em todos os dispositivos no locatário. Unidade em porcentagem. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthAppImpact"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthAppImpact",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "isForegroundApp": true,
  "batteryUsagePercentage": "4.2"
}
```




