---
title: tipo de recurso onenoteOperation
description: O status de determinadas operações demoradas do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 500a4c20583f6af9cc8bacf98dd4de60354f0ab2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522341"
---
# <a name="onenoteoperation-resource-type"></a>tipo de recurso onenoteOperation

Namespace: microsoft.graph

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
|id|cadeia de caracteres|A ID da operação. Somente leitura.|
|lastActionDateTime| DateTimeOffset |A hora da última ação da operação.|
|resourceId|cadeia de caracteres|A ID do recurso.|
|resourceLocation|cadeia de caracteres|O URI do recurso para o objeto. Por exemplo, o URI do recurso para uma página ou seção copiada. |
|status|cadeia de caracteres|O status atual da operação: `notstarted` , `running` , `completed` ,`failed` |
|percentComplete|cadeia de caracteres|A porcentagem concluída da operação se a operação ainda estiver em `running` status

## <a name="relationships"></a>Relações
Nenhuma


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Operação get](../api/onenoteoperation-get.md) | [onenoteOperation](onenoteoperation.md) |Obter o status da operação. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
