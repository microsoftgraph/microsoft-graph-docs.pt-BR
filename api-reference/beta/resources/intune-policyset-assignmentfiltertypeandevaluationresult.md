---
title: Tipo de recurso assignmentFilterTypeAndEvaluationResult
description: Representa o tipo de filtro e o resultado de avaliação do filtro.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4378df019720583a5851792d5c5c8003be9fd985
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074931"
---
# <a name="assignmentfiltertypeandevaluationresult-resource-type"></a>Tipo de recurso assignmentFilterTypeAndEvaluationResult

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o tipo de filtro e o resultado de avaliação do filtro.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignmentFilterType|[deviceAndAppManagementAssignmentFilterType](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|Representa o tipo de filtro. Os valores possíveis são: `none`, `include`, `exclude`.|
|evaluationResult|[assignmentFilterEvaluationResult](../resources/intune-policyset-assignmentfilterevaluationresult.md)|Representa o resultado de evalaution do filtro. Os possíveis valores são: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterTypeAndEvaluationResult",
  "assignmentFilterType": "String",
  "evaluationResult": "String"
}
```



