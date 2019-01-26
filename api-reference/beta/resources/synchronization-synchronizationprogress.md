---
title: tipo de recurso de synchronizationProgress
description: Representa o progresso de um synchronizationJob rumo à conclusão.
localization_priority: Normal
ms.openlocfilehash: 39351f07720d44679675396f9e995f5e78e25fcc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572742"
---
# <a name="synchronizationprogress-resource-type"></a>tipo de recurso de synchronizationProgress

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o progresso de um [synchronizationJob](synchronization-synchronizationjob.md) rumo à conclusão.

## <a name="properties"></a>Propriedades

| Propriedade                              | Tipo      | Descrição    |
|:--------------------------------------|:----------|:---------------|
|completedUnits|Int32|O numerador de uma proporção de progresso; o número de unidades de alterações já processadas.|
|progressObservationDateTime|DateTimeOffset|A hora de uma observação de progresso como um deslocamento em minutos de UTC.|
|totalUnits|Int32|Denominador de uma proporção de progresso; um número de unidades de alterações a serem processados para realizar a sincronização.|
|unidades|String|Uma descrição opcional das unidades.|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationProgress"
}-->

```json
{
  "completedUnits": 1025,
  "progressObservationDateTime": "2017-10-10T17:00:00Z",
  "totalUnits": 3024,
  "units": "pages"
}

```

<!-- uuid: 15571993-7e2f-4842-84d5-01ceb67cdc05
20185-08-14 22:30:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationprogress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
