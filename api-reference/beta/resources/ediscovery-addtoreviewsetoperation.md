---
title: Tipo de recurso addToReviewSetOperation
description: Adiciona os resultados de uma sourceCollection a um reviewSet
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d7323fbd6d2d068888d556328fc3ea4e399ab2fe
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446181"
---
# <a name="addtoreviewsetoperation-resource-type"></a>Tipo de recurso addToReviewSetOperation

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma operação para adicionar [uma sourceCollection](../resources/ediscovery-sourcecollection.md) a um [reviewSet](../resources/ediscovery-reviewset.md).

Herda de [caseOperation](../resources/ediscovery-caseoperation.md).

## <a name="methods"></a>Methods

Nenhum.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| A ação de caso dessa entidade sempre será `addToReviewSet` . Somente leitura. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|completedDateTime|DateTimeOffset|A data e a hora em que a operação foi concluída. Somente leitura. Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a operação. Somente leitura. Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)|
|createdDateTime|DateTimeOffset|A data e a hora em que a operação foi iniciada. Somente leitura. Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)|
|id|String| A ID da operação. Somente leitura. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|percentProgress|Int32|O progresso da operação. Somente leitura. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|resultInfo|[resultInfo](../resources/resultinfo.md)|Contém informações de resultados específicas de falha e sucesso. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|O status da operação de caso. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md). Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

### <a name="datacollectionscope-values"></a>valores dataCollectionScope

|Member|Descrição|
|:----|-----------|
|allVersions|Inclua todas as versões de arquivos de sites.|
|linkedFiles|Inclua **anexo de nuvem** com emails na coleção.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|reviewSet|[microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)| O conjunto de revisão ao qual os itens correspondentes à consulta da coleção de origem são adicionados. |
|sourceCollection|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourceCollection.md)| A sourceCollection de onde os itens estão sendo adicionados. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.addToReviewSetOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.addToReviewSetOperation",
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
