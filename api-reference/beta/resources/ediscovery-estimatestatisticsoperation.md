---
title: Tipo de recurso estimateStatisticsOperation
description: Representa a operação que lida com a estimativa da contagem e do tamanho de uma coleção de origem.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e816ba01d4bb648a8e78b5b96369236f63fb163e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445928"
---
# <a name="estimatestatisticsoperation-resource-type"></a>Tipo de recurso estimateStatisticsOperation

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a operação que lida com a estimativa da contagem e do tamanho de [uma sourceCollection](../resources/ediscovery-sourcecollection.md). Para obter detalhes, [consulte Coletar dados para uma ocorrência em Descoberta Avançada de eDiscovery](/microsoft-365/compliance/collecting-data-for-ediscovery).

Herda de [caseOperation](../resources/ediscovery-caseoperation.md).

## <a name="methods"></a>Methods

Nenhum.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|microsoft.graph.ediscovery.caseAction| O tipo de operação. A ação de caso dessa entidade sempre será `estimateStatistics` . Somente leitura. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|completedDateTime|DateTimeOffset|A data e a hora em que a operação foi concluída. Somente leitura. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a operação. Somente leitura. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|createdDateTime|DateTimeOffset|A data e a hora em que a operação foi iniciada. Somente leitura. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|id|String| A ID da operação. Somente leitura. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|indexedItemCount|Int64|A contagem estimada de itens para **o sourceCollection** que corresponderam à consulta de conteúdo.|
|indexedItemsSize|Int64|O tamanho estimado de itens para **o sourceCollection** que corresponderam à consulta de conteúdo.|
|mailboxCount|Int32|O número de caixas de correio que tiveram visitas de pesquisa.|
|percentProgress|Int32|O progresso da operação. Somente leitura. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|resultInfo|[resultInfo](../resources/resultinfo.md)|Contém informações de resultados específicas de falha e sucesso. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|siteCount|Int32|O número de caixas de correio que tiveram visitas de pesquisa.|
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|O status da operação de caso. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md). Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|
|unindexedItemCount|Int64|A contagem estimada de itens não índicedos para a coleção.|
|unindexedItemsSize|Int64|O tamanho estimado de itens não índicedos para a coleção.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|sourceCollection|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Coleção eDiscovery, comumente conhecida como pesquisa.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.estimateStatisticsOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/operations/$entity",
    "@odata.type": "#microsoft.graph.ediscovery.estimateStatisticsOperation",
    "createdDateTime": "2021-01-12T18:47:23.3974907Z",
    "completedDateTime": "2021-01-12T18:47:51.1461805Z",
    "percentProgress": 100,
    "status": "succeeded",
    "action": "estimateStatistics",
    "id": "82edd40e182a464fa02c24a36fa94873",
    "indexedItemCount": 2,
    "indexedItemsSize": 39276,
    "unindexedItemCount": 0,
    "unindexedItemsSize": 0,
    "mailboxCount": 1,
    "siteCount": 0,
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null,
            "userPrincipalName": "admin@contoso.com"
        }
    }
}
```
