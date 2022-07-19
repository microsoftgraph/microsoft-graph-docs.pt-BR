---
title: Tipo de recurso ediscoveryIndexOperation
description: Representa o processo de indexação de fontes de dados, incluindo custodiantes e fontes de dados não custodiantes.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 59e90a1a66ee26b12685c6e91cf60c4989d0c377
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837538"
---
# <a name="ediscoveryindexoperation-resource-type"></a>Tipo de recurso ediscoveryIndexOperation

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o processo de indexação de fontes de dados, incluindo custodiantes e fontes de dados não custodiantes.

Herda de [caseOperation](../resources/security-caseoperation.md).

## <a name="methods"></a>Métodos

Nenhum.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|[microsoft.graph.security.caseAction](../resources/security-caseoperation.md#caseaction-values)| O tipo de ação que a operação representa. Os valores possíveis são: `addToReviewSet`,`applyTags`,`contentExport`,,`convertToPdf`,`estimateStatistics``purgeData`|
|completedDateTime|DateTimeOffset| A data e a hora em que a operação foi concluída. |
|createdBy|[identitySet](../resources/identityset.md)| O usuário que criou a operação. |
|createdDateTime|DateTimeOffset| A data e a hora em que a operação foi criada. |
|id|Cadeia de caracteres| A ID da operação. Somente leitura. |
|percentProgress|Int32| O progresso da operação. |
|resultInfo|[resultInfo](../resources/resultinfo.md)| Contém informações de resultado específicas de êxito e falha. |
|status|[microsoft.graph.security.caseOperationStatus](../resources/security-caseoperation.md#caseoperationstatus-values)| O status da operação de caso. Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryIndexOperation",
  "baseType": "microsoft.graph.security.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryIndexOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "percentProgress": "Integer",
  "status": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```

