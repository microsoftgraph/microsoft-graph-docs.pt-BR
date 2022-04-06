---
title: Tipo de recurso purgeDataOperation
description: Representa uma operação para excluir permanentemente dados em uma sourceCollection. Atualmente, a operação tem escopo para Microsoft Teams apenas mensagens.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 5562658c40831cea39922dfd5d1e1edc1d214392
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608407"
---
# <a name="purgedataoperation-resource-type"></a>Tipo de recurso purgeDataOperation

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma operação para excluir permanentemente dados em uma sourceCollection. No momento, essa operação tem escopo para Microsoft Teams apenas mensagens; mais fontes de dados estarão no escopo no futuro.

Herda de [caseOperation](../resources/ediscovery-caseoperation.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| O tipo de ação que a operação representa. Os valores possíveis são: `addToReviewSet`,`applyTags`,`contentExport`,`convertToPdf`,,`estimateStatistics`,`purgeData`.|
|completedDateTime|DateTimeOffset| A data e a hora em que a operação foi concluída. |
|createdBy|[identitySet](../resources/identityset.md)| O usuário que criou a operação. |
|createdDateTime|DateTimeOffset| A data e a hora em que a operação foi criada. |
|id|Cadeia de caracteres| A ID da operação. Somente leitura. |
|percentProgress|Int32| O progresso da operação. |
|resultInfo|[resultInfo](../resources/resultinfo.md)| Contém informações de resultados específicas de falha e sucesso. |
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)| O status da operação de caso. Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.purgeDataOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.purgeDataOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```
