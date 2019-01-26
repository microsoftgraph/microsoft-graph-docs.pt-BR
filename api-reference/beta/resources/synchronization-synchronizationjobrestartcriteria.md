---
title: tipo de recurso de synchronizationJobRestartCriteria
description: 'Define o escopo do [synchronizationJob: reiniciar](../api/synchronization_synchronizationjob_restart.md) ação.'
localization_priority: Normal
ms.openlocfilehash: 960bfa56d0bb6921ca971722d894d1b837bfab49
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572301"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>tipo de recurso de synchronizationJobRestartCriteria

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define o escopo do [synchronizationJob: reiniciar](../api/synchronization-synchronizationjob-restart.md) ação.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|resetScope|String| Combinação de separada por vírgulas dos seguintes valores: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`. Uso `Full` se desejar que todas as opções.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjobrestartcriteria.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
