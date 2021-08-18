---
title: Tipo de recurso userExperienceAnalyticsInsight
description: O insight de análise de experiência do usuário é a recomendação para melhorar a pontuação de análise da experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 091ac9a6513dc97c80560009b219a5c57d3da14a2808fac1477607f98d5aae47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54213120"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a>Tipo de recurso userExperienceAnalyticsInsight

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O insight de análise de experiência do usuário é a recomendação para melhorar a pontuação de análise da experiência do usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userExperienceAnalyticsMetricId|Cadeia de caracteres|O identificador exclusivo do insight de análise de experiência do usuário.|
|insightId|Cadeia de caracteres|O identificador exclusivo do insight de análise de experiência do usuário.|
|values|[Coleção userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)|O valor do insight de análise da experiência do usuário.|
|severity|[userExperienceAnalyticsInsightSeverity](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|O valor do insight de análise da experiência do usuário. Os valores possíveis são: `none`, `informational`, `warning`, `error`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
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
```




