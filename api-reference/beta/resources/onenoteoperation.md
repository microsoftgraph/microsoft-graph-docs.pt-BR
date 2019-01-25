---
title: Tipo de recurso onenoteOperation
description: O status de determinadas operações demoradas do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 146a1b1d9a51cc541e06fd789f987a2d39dff48a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512847"
---
# <a name="onenoteoperation-resource-type"></a>Tipo de recurso onenoteOperation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O status de determinadas operações demoradas do OneNote.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |A hora de início da operação.|
|erro|[onenoteOperationError](onenoteoperationerror.md)|O erro retornado pela operação.|
|id|string|A id da operação. Somente leitura.|
|lastActionDateTime| DateTimeOffset |A hora da última ação da operação.|
|resourceId|string|A id do recurso.|
|resourceLocation|string|O URI de recurso do objeto. Por exemplo, o URI de recurso para uma seção ou página copiada. |
|status|string|O status atual da operação: `notstarted`, `running`, `completed`, `failed` |
|percentComplete|string|A porcentagem concluída da operação se a operação ainda estiver com um status `running`

## <a name="relationships"></a>Relações
Nenhum


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get operation](../api/onenoteoperation-get.md) | [onenoteOperation](onenoteoperation.md) |Obter o status atual da operação. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
