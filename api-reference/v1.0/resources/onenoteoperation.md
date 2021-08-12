---
title: Tipo de recurso do onenoteOperation
description: O status de determinadas operações de OneNote de longo prazo.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: dd7d6cfc797416d0cc8922dac8305617bc46c4c8d26e0e138551a0f855cadcbb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146444"
---
# <a name="onenoteoperation-resource-type"></a>Tipo de recurso do onenoteOperation

Namespace: microsoft.graph

O status de determinadas operações de OneNote de longo prazo.

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
|resourceId|string|A ID do recurso.|
|resourceLocation|string|O URI do recurso do objeto. Por exemplo, o URI de recurso para uma página ou seção copiada. |
|status|operationStatus|O status atual da operação: `NotStarted` , `Running` , , `Completed` `Failed` . |
|percentComplete|string|A porcentagem de operação será concluída se a operação ainda estiver em `running` status.|

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

