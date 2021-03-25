---
title: Tipo de recurso assignmentFilterEvaluationSummary
description: Representar resumo de resultados para avaliação de filtro de atribuição
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05c9a3eabd22e7e22a6d74229b7aa47901e05db6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155978"
---
# <a name="assignmentfilterevaluationsummary-resource-type"></a>Tipo de recurso assignmentFilterEvaluationSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representar resumo de resultados para avaliação de filtro de atribuição

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignmentFilterId|Cadeia de caracteres|Identificador exclusivo do objeto de filtro de atribuição|
|assignmentFilterLastModifiedDateTime|DateTimeOffset|A hora em que o filtro de atribuição foi modificado pela última vez.|
|assignmentFilterDisplayName|Cadeia de caracteres|O nome definido pelo administrador para filtro de atribuição.|
|assignmentFilterPlatform|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|A plataforma para a qual esse filtro de atribuição é criado. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|evaluationResult|[assignmentFilterEvaluationResult](../resources/intune-policyset-assignmentfilterevaluationresult.md)|Resultado da avaliação do filtro de atribuição. Os possíveis valores são: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.|
|evaluationDateTime|DateTimeOffset|O filtro de atribuição de hora foi avaliado.|
|assignmentFilterType|[deviceAndAppManagementAssignmentFilterType](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|Indique o tipo de filtro incluir ou excluir. Os valores possíveis são: `none`, `include`, `exclude`.|
|assignmentFilterTypeAndEvaluationResults|[coleção assignmentFilterTypeAndEvaluationResult](../resources/intune-policyset-assignmentfiltertypeandevaluationresult.md)|Uma coleção de tipos de filtro e seus resultados de avaliação correspondentes.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationSummary",
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
```




