---
title: Tipo de recurso tagOperation
description: Representa a operação que lida com a aplicação de marcas a documentos em um conjunto de revisão com base em uma consulta de conjunto de revisão.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 2af9b255e643a46f5f065b3caf62fda0ae9967a4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445943"
---
# <a name="tagoperation-resource-type"></a>Tipo de recurso tagOperation

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a operação que lida com a aplicação de marcas a documentos em um conjunto de revisão com base em uma consulta de conjunto de revisão.

Herda de [caseOperation](../resources/ediscovery-caseoperation.md).

## <a name="methods"></a>Methods

Nenhum.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| A ação de caso dessa entidade sempre será `applyTags` . Somente leitura. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|completedDateTime|DateTimeOffset|A data e a hora em que a operação foi concluída. Somente leitura. Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a operação. Somente leitura. Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)|
|createdDateTime|DateTimeOffset|A data e a hora em que a operação foi iniciada. Somente leitura. Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)|
|id|String| A ID da operação. Somente leitura. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|percentProgress|Int32|O progresso da operação. Somente leitura. Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)|
|resultInfo|[resultInfo](../resources/resultinfo.md)|Contém informações de resultados específicas de falha e sucesso. Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)|
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|O status da operação de caso. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md). Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.tagOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.tagOperation",
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
