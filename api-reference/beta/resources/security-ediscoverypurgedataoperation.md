---
title: Tipo de recurso ediscoveryPurgeDataOperation
description: Representa o processo de limpeza de dados de uma pesquisa de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e186c2bbca4a1b9b5cfc0cc2d00e476ae5a35aa1
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945037"
---
# <a name="ediscoverypurgedataoperation-resource-type"></a>Tipo de recurso ediscoveryPurgeDataOperation

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o processo de limpeza de dados de uma pesquisa de Descoberta Eletrônica.

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
  "@odata.type": "microsoft.graph.security.ediscoveryPurgeDataOperation",
  "baseType": "microsoft.graph.security.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryPurgeDataOperation",
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

