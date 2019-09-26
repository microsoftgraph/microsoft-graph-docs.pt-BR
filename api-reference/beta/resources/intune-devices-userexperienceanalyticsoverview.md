---
title: tipo de recurso userExperienceAnalyticsOverview
description: A entidade visão geral da análise da experiência do usuário contém a pontuação geral e as pontuações e os resultados de cada métrica de todas as categorias.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 11c7bbe64b1495a9e6cb0b8ac144d1afb539789f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196669"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a>tipo de recurso userExperienceAnalyticsOverview

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade visão geral da análise da experiência do usuário contém a pontuação geral e as pontuações e os resultados de cada métrica de todas as categorias.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .|
|[Atualizar userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da visão geral da análise da experiência do usuário.|
|overallScore|Int32|A pontuação geral da análise da experiência do usuário.|
|deviceBootPerformanceOverallScore|Int32|A pontuação geral do desempenho de inicialização do dispositivo analítico da experiência do usuário.|
|bestPracticesOverallScore|Int32|A pontuação geral das práticas recomendadas de análise da experiência do usuário.|
|insights|coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)|A experiência do usuário do Analytics insights.|
|estado|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de integridade atual da categoria de análise da experiência do usuário. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

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
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "String",
      "insightId": "String",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "String"
    }
  ],
  "state": "String"
}
```



