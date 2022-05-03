---
title: Tipo de recurso printOperation
description: Representa uma operação de Impressão Universal de execução longa. Classe base para tipos de operação, como printerCreateOperation.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5e3d53d9fbdc5fbb4dd1bda2aa477581df5c838e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176665"
---
# <a name="printoperation-resource-type"></a>Tipo de recurso printOperation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma operação de Impressão Universal de execução longa. Classe base para tipos de operação, como [printerCreateOperation](printercreateoperation.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter operação](../api/printoperation-get.md) | [printOperation](printoperation.md) | Recupere uma operação de execução longa dentro do locatário do usuário ou do aplicativo atual. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador da operação. Somente leitura.|
|status|[printOperationStatus](printoperationstatus.md)|O status da operação. Somente leitura.|
|createdDateTime|DateTimeOffset|O DateTimeOffset quando a operação foi criada. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


