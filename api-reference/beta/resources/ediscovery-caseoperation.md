---
title: Tipo de recurso caseOperation
description: Uma entidade abstrata que representa um processo de Descoberta eDiscovery de longa duração.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b94aeba03a49f2c49cbf991f0046422a18b20b50
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446174"
---
# <a name="caseoperation-resource-type"></a>Tipo de recurso caseOperation

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma entidade abstrata que representa um processo de Descoberta eDiscovery de longa duração. Ele contém um conjunto comum de propriedades que são compartilhadas entre entidades herdadas.  Entidades derivadas de **caseOperation** incluem:

- [caseExportOperation](../resources/ediscovery-caseexportoperation.md)
- [tagOperation](../resources/ediscovery-tagoperation.md)
- [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md)

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Methods

Nenhum.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| O tipo de ação que a operação representa. Os valores possíveis são: `addToReviewSet` , `applyTags` , `contentExport` , `convertToPdf``estimateStatistics`|
|completedDateTime|DateTimeOffset| A data e a hora em que a operação foi concluída. |
|createdBy|[identitySet](../resources/identityset.md)| O usuário que criou a operação. |
|createdDateTime|DateTimeOffset| A data e a hora em que a operação foi criada. |
|id|String| A ID da operação. Somente leitura. |
|percentProgress|Int32| O progresso da operação. |
|resultInfo|[resultInfo](../resources/resultinfo.md)| Contém informações de resultados específicas de falha e sucesso. |
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)| O status da operação de caso. Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

### <a name="caseaction-values"></a>valores caseAction

|Member|Descrição|
|:----|-----------|
| addToReviewSet | A operação representa a adição de dados a um conjunto de revisão de uma coleção eDiscovery. |
| applyTags | A operação representa documentos de marcação em massa em um conjunto de revisão para a consulta do conjunto de revisão especificado. |
| contentExport | A operação representa uma exportação de conteúdo de um conjunto de revisão. |
| convertToPdf | A operação representa a conversão de documentos em PDFs com redação. |
| estimateStatistics  | A operação representa a pesquisa em serviços do Microsoft 365, como Exchange, SharePoint e OneDrive para empresas. |

### <a name="caseoperationstatus-values"></a>valores caseOperationStatus

|Member|Descrição|
|:----|-----------|
| notStarted | A operação ainda não foi iniciada. |
| submissionFailed | Falha no envio da operação. |
| running | A operação está em execução no momento. |
| bem-sucedido | A operação foi concluída com êxito sem erros. |
| partiallySucceededed | A operação foi concluída, mas houve erros - Consulte [resultInfo para](../resources/resultinfo.md) obter detalhes de erro. |
| failed | Falha na operação - Consulte informações de resultados para obter detalhes de erro. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseOperation",
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
