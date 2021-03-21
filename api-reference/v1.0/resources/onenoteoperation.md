---
title: Tipo de recurso do onenoteOperation
description: O status de determinadas operações do OneNote de longa duração.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 146cfec00c630fc0abde326a57374549d7b2d378
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961948"
---
# <a name="onenoteoperation-resource-type"></a>Tipo de recurso do onenoteOperation

Namespace: microsoft.graph

O status de determinadas operações do OneNote de longa duração.

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
|id|cadeia de caracteres|A id da operação. Somente leitura.|
|lastActionDateTime| DateTimeOffset |A hora da última ação da operação.|
|resourceId|cadeia de caracteres|A ID do recurso.|
|resourceLocation|cadeia de caracteres|O URI do recurso do objeto. Por exemplo, o URI de recurso para uma página ou seção copiada. |
|status|operationStatus|O status atual da operação: `NotStarted` , `Running` , , `Completed` `Failed` . |
|percentComplete|cadeia de caracteres|A porcentagem de operação será concluída se a operação ainda estiver em `running` status.|

## <a name="relationships"></a>Relações
Nenhuma


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter operação](../api/onenoteoperation-get.md) | [onenoteOperation](onenoteoperation.md) |Obter o status da operação. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

