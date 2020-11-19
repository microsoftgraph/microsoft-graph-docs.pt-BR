---
title: tipo de recurso userExperienceAnalyticsRegressionSummary
description: O resumo de regressão da análise da experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 23db3acb1fde40f8f43e9049a5dc82c120cdbdb1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256408"
---
# <a name="userexperienceanalyticsregressionsummary-resource-type"></a>tipo de recurso userExperienceAnalyticsRegressionSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O resumo de regressão da análise da experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userExperienceAnalyticsRegressionSummary](../api/intune-devices-userexperienceanalyticsregressionsummary-get.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) .|
|[Atualizar userExperienceAnalyticsRegressionSummary](../api/intune-devices-userexperienceanalyticsregressionsummary-update.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) .|
|[função summarizeDeviceRegressionPerformance](../api/intune-devices-userexperienceanalyticsregressionsummary-summarizedeviceregressionperformance.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do Resumo de regressão da análise da experiência do usuário.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|modelRegression|coleção [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Os valores de métrica para a regressão do modelo de análise da experiência do usuário.|
|manufacturerRegression|coleção [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Os valores de métrica para a regressão do fabricante da análise da experiência do usuário.|
|operatingSystemRegression|coleção [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Os valores de métrica para a regressão do sistema operacional de análise da experiência do usuário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsRegressionSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "String (identifier)"
}
```




