---
title: tipo de recurso de convertIdResult
description: O resultado de uma conversão de formato de ID realizada pela função translateExchangeIds.
localization_priority: Normal
ms.openlocfilehash: db28172d009ee8a8a39b7e02733d893dc20a81e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516522"
---
# <a name="convertidresult-resource-type"></a>tipo de recurso de convertIdResult

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O resultado de uma conversão de formato de ID realizada pela função [translateExchangeIds](../api/user-translateexchangeids.md) .

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| SourceId | String | O identificador que foi convertido. Esse valor é o identificador original, não convertido. |
| Alvo | String | O identificador convertido. Este valor não estiver presente, se a conversão falhou. |
| errorDetails | [Erro genérico](genericerror.md) | Um objeto de erro que indica o motivo da falha de conversão. Este valor não estiver presente, se a conversão foi bem-sucedida. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/convertidresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
