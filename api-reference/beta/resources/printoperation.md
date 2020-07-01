---
title: tipo de recurso de multioperação
description: Representa uma operação de impressão universal de execução longa. Classe base para tipos de operação, como printerCreateOperation.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7b8f147106c6914fe8fbbb404ca0c78210c02026
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007145"
---
# <a name="printoperation-resource-type"></a>tipo de recurso de multioperação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma operação de impressão universal de execução longa. Classe base para tipos de operação, como [printerCreateOperation](printercreateoperation.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Operação get](../api/printoperation-get.md) | [Operação de reoperação](printoperation.md) | Recupere uma operação de execução longa dentro do usuário atual ou do locatário do aplicativo. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador da operação. Somente leitura.|
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