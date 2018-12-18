---
title: Tipo de recurso onenoteOperation
description: O status de determinadas operações demoradas do OneNote.
author: Jewan-microsoft
ms.openlocfilehash: bbb7b9457ce5a3d7ba9faf45d893ae86cdfd8b32
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326905"
---
# <a name="onenoteoperation-resource-type"></a>Tipo de recurso onenoteOperation

O status de determinadas operações demoradas do OneNote.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.operation",
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
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
