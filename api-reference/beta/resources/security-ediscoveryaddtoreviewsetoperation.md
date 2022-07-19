---
title: Tipo de recurso ediscoveryAddToReviewSetOperation
description: Adiciona os resultados de uma sourceCollection a um reviewSet
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 7e16dc269d212517465c3492dcbe30b9fd3de7d4
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838630"
---
# <a name="ediscoveryaddtoreviewsetoperation-resource-type"></a>Tipo de recurso ediscoveryAddToReviewSetOperation

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma operação para adicionar [um eDiscoverySearch](../resources/security-ediscoverysearch.md) a [um eDiscoveryReviewSet](../resources/security-ediscoveryreviewset.md).

Herda de [caseOperation](../resources/security-caseoperation.md).

## <a name="methods"></a>Métodos
Nenhum.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|microsoft.graph.security.caseAction| O tipo de ação que a operação representa. Os valores possíveis são: `addToReviewSet`,`applyTags`,`contentExport`,,`convertToPdf`,`estimateStatistics``purgeData`|
|completedDateTime|DateTimeOffset| A data e a hora em que a operação foi concluída. |
|createdBy|[identitySet](../resources/identityset.md)| O usuário que criou a operação. |
|createdDateTime|DateTimeOffset| A data e a hora em que a operação foi criada. |
|id|Cadeia de caracteres| A ID da operação. Somente leitura. |
|percentProgress|Int32| O progresso da operação. |
|resultInfo|[resultInfo](../resources/resultinfo.md)| Contém informações de resultado específicas de êxito e falha. |
|status|microsoft.graph.security.caseOperationStatus| O status da operação de caso. Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|reviewSet|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Conjunto de revisão de Descoberta Eletrônica ao qual os itens correspondentes à consulta da coleção de origem são adicionados.|
|search|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Pesquisa de Descoberta Eletrônica que é adicionada ao conjunto de revisão.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryAddToReviewSetOperation",
  "baseType": "microsoft.graph.security.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryAddToReviewSetOperation",
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

