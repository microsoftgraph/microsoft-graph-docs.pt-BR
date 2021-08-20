---
title: Tipo de recurso assignmentFilterStatusDetails
description: Represente detalhes de status para dispositivo e carga e todos os filtros aplicados associados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d306c1b0d05e2418653e37737c33f52514be39c4
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266181"
---
# <a name="assignmentfilterstatusdetails-resource-type"></a>Tipo de recurso assignmentFilterStatusDetails

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Represente detalhes de status para dispositivo e carga e todos os filtros aplicados associados.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|managedDeviceId|Cadeia de caracteres|Identificador exclusivo do objeto device.|
|payloadId|Cadeia de caracteres|Identificador exclusivo do objeto de carga.|
|userId|Cadeia de caracteres|Identificador exclusivo do objeto UserId. Pode ser nulo|
|deviceProperties|Coleção [keyValuePair](../resources/intune-policyset-keyvaluepair.md)|Propriedades do dispositivo usadas para avaliação de filtro durante o tempo de check-in do dispositivo.|
|evalutionSummaries|[coleção assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md)|Resumos de resultados de avaliação para cada filtro associado ao dispositivo e à carga|

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
      "assignmentFilterType": "String",
      "assignmentFilterTypeAndEvaluationResults": [
        {
          "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
          "assignmentFilterType": "String",
          "evaluationResult": "String"
        }
      ]
    }
  ]
}
```




