---
title: Tipo de recurso userExperienceAnalyticsOverview
description: A entidade de visão geral da análise de experiência do usuário contém a pontuação geral e as pontuações e percepções de cada métrica de todas as categorias.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb19080f06848bb2279685eda7eabadb70bb1458
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687975"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a>Tipo de recurso userExperienceAnalyticsOverview

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de visão geral da análise de experiência do usuário contém a pontuação geral e as pontuações e percepções de cada métrica de todas as categorias.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|Ler propriedades e relações do [objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)|
|[Atualizar userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da visão geral da análise de experiência do usuário.|
|overallScore|Int32|A pontuação geral da análise de experiência do usuário.|
|deviceBootPerformanceOverallScore|Int32|A pontuação geral do desempenho geral de inicialização do dispositivo de análise de experiência do usuário.|
|bestPracticesOverallScore|Int32|A pontuação geral das práticas recomendadas da análise da experiência do usuário.|
|workFromAnywhereOverallScore|Int32|A pontuação geral da análise de experiência do usuário Work From Anywhere.|
|appHealthOverallScore|Int32|A pontuação geral de saúde geral do aplicativo de análise de experiência do usuário.|
|resourcePerformanceOverallScore|Int32|A pontuação geral do desempenho geral do recurso de análise de experiência do usuário.|
|batteryHealthOverallScore|Int32|A pontuação geral da bateria de análise de experiência do usuário.|
|insights|[Coleção userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)|As percepções de análise de experiência do usuário.|
|estado|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da visão geral da análise da experiência do usuário. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|deviceBootPerformanceHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da categoria de análise de experiência do usuário 'BootPerformance'. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|bestPracticesHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da categoria de análise de experiência do usuário "BestPractices". Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|workFromAnywhereHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da categoria de análise de experiência do usuário 'WorkFromAnywhere'. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|appHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da categoria de análise de experiência do usuário "BestPractices". Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|resourcePerformanceHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da categoria de análise de experiência do usuário 'ResourcePerformance'. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|batteryHealthHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da categoria de análise de experiência do usuário 'BatteryHealth'. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "String (identifier)",
  "overallScore": 1024,
  "deviceBootPerformanceOverallScore": 1024,
  "bestPracticesOverallScore": 1024,
  "workFromAnywhereOverallScore": 1024,
  "appHealthOverallScore": 1024,
  "resourcePerformanceOverallScore": 1024,
  "batteryHealthOverallScore": 1024,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "String",
      "insightId": "String",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "4.2"
        }
      ],
      "severity": "String"
    }
  ],
  "state": "String",
  "deviceBootPerformanceHealthState": "String",
  "bestPracticesHealthState": "String",
  "workFromAnywhereHealthState": "String",
  "appHealthState": "String",
  "resourcePerformanceHealthState": "String",
  "batteryHealthHealthState": "String"
}
```



