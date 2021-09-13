---
title: Tipo de recurso assignmentFilterEvaluationSummary
description: Representar resumo de resultados para avaliação de filtro de atribuição
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 47b38a462439d0b23ae2bfb51f56a41c3e272699
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100964"
---
# <a name="assignmentfilterevaluationsummary-resource-type"></a>Tipo de recurso assignmentFilterEvaluationSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representar resumo de resultados para avaliação de filtro de atribuição

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignmentFilterId|Cadeia de Caracteres|Identificador exclusivo do objeto de filtro de atribuição|
|assignmentFilterLastModifiedDateTime|DateTimeOffset|A hora em que o filtro de atribuição foi modificado pela última vez.|
|assignmentFilterDisplayName|Cadeia de Caracteres|O nome definido pelo administrador para filtro de atribuição.|
|assignmentFilterPlatform|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|A plataforma para a qual esse filtro de atribuição é criado. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
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



