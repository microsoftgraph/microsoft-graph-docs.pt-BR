---
title: Tipo de recurso userExperienceAnalyticsRegressionSummary
description: Resumo da regressão de análise de experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9b716f279fc928f513ccfd874fc25933a52fa7c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789909"
---
# <a name="userexperienceanalyticsregressionsummary-resource-type"></a>Tipo de recurso userExperienceAnalyticsRegressionSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo da regressão de análise de experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userExperienceAnalyticsRegressionSummary](../api/intune-devices-userexperienceanalyticsregressionsummary-get.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsRegressionSummary.](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|
|[Atualizar userExperienceAnalyticsRegressionSummary](../api/intune-devices-userexperienceanalyticsregressionsummary-update.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsRegressionSummary.](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|
|[função summarizeDeviceRegressionPerformance](../api/intune-devices-userexperienceanalyticsregressionsummary-summarizedeviceregressionperformance.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do resumo de regressão de análise de experiência do usuário.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|modelRegression|[Coleção userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Os valores métricos para a regressão do modelo de análise de experiência do usuário.|
|manufacturerRegression|[Coleção userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Os valores métricos para a regressão do fabricante de análise de experiência do usuário.|
|operatingSystemRegression|[Coleção userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Os valores métricos da regressão do sistema operacional de análise de experiência do usuário.|

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



