---
title: Tipo de recurso ediscoveryEstimateOperation
description: Representa o processo de estimativa de estatísticas (contagem de itens, tamanho e número de locais) de uma pesquisa de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f49f6356af89166ed384a56c0e4f3fe8bb4d553a
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945053"
---
# <a name="ediscoveryestimateoperation-resource-type"></a>Tipo de recurso ediscoveryEstimateOperation

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o processo de estimativa de estatísticas (contagem de itens, tamanho e número de locais) de uma pesquisa de Descoberta Eletrônica.

Herda de [caseOperation](../resources/security-caseoperation.md).

## <a name="methods"></a>Métodos
Nenhum.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|String| O tipo de ação que a operação representa. Os valores possíveis são: `addToReviewSet`,`applyTags`,`contentExport`,,`convertToPdf`,`estimateStatistics``purgeData`|
|completedDateTime|DateTimeOffset|A data e a hora em que a operação foi concluída. Somente leitura. |
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a operação. Somente leitura. |
|createdDateTime|DateTimeOffset|A data e a hora em que a operação foi iniciada. Somente leitura.|
|id|Cadeia de caracteres| A ID da operação. Somente leitura.|
|indexedItemCount|Int64|A contagem estimada de itens para **a pesquisa** que correspondeu à consulta de conteúdo.|
|indexedItemsSize|Int64|O tamanho estimado de itens para **a pesquisa** que correspondeu à consulta de conteúdo.|
|mailboxCount|Int32|O número de caixas de correio que tiveram ocorrências de pesquisa.|
|percentProgress|Int32|O progresso da operação. Somente leitura. |
|resultInfo|[resultInfo](../resources/resultinfo.md)|Contém informações de resultado específicas de êxito e falha. |
|siteCount|Int32|O número de caixas de correio que tiveram ocorrências de pesquisa.|
|status|Cadeia de caracteres| O status da operação de caso. Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|
|unindexedItemCount|Int64|A contagem estimada de itens não indexados para a coleção.|
|unindexedItemsSize|Int64|O tamanho estimado de itens não indexados para a coleção.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|search|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Pesquisa de Descoberta Eletrônica.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryEstimateOperation",
  "baseType": "microsoft.graph.security.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryEstimateOperation",
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
  },
  "indexedItemCount": "Integer",
  "indexedItemsSize": "Integer",
  "unindexedItemCount": "Integer",
  "unindexedItemsSize": "Integer",
  "mailboxCount": "Integer",
  "siteCount": "Integer"
}
```

