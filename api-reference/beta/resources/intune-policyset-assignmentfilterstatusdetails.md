---
title: Tipo de recurso assignmentFilterStatusDetails
description: Representam detalhes de status para o dispositivo e a carga e todos os filtros aplicados associados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a376b1ff3d554753120860f1d3541f7952dd6130
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160160"
---
# <a name="assignmentfilterstatusdetails-resource-type"></a>Tipo de recurso assignmentFilterStatusDetails

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representam detalhes de status para o dispositivo e a carga e todos os filtros aplicados associados.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|managedDeviceId|String|Identificador exclusivo do objeto de dispositivo.|
|payloadId|String|Identificador exclusivo do objeto de carga.|
|userId|Cadeia de caracteres|Identificador exclusivo do objeto UserId. Pode ser nulo|
|deviceProperties|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Propriedades do dispositivo usadas para avaliação de filtro durante o tempo de check-in do dispositivo.|
|evalutionSummaries|[Coleção assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md)|Resumos de resultados de avaliação para cada filtro associado ao dispositivo e ao conteúdo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterStatusDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterStatusDetails",
  "managedDeviceId": "String",
  "payloadId": "String",
  "userId": "String",
  "deviceProperties": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "evalutionSummaries": [
    {
      "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary",
      "assignmentFilterId": "String",
      "assignmentFilterLastModifiedDateTime": "String (timestamp)",
      "assignmentFilterDisplayName": "String",
      "assignmentFilterPlatform": "String",
      "evaluationResult": "String",
      "evaluationDateTime": "String (timestamp)",
      "assignmentFilterType": "String"
    }
  ]
}
```




