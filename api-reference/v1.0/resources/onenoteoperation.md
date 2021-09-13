---
title: Tipo de recurso do onenoteOperation
description: O status de determinadas operações de OneNote de longo prazo.
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: ef25b94bb02ffaf721e7861eecacdd37c4c85e9f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118036"
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

