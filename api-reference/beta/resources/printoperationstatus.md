---
title: tipo de recurso printOperationStatus
description: Representa o status atual de uma operação de impressão universal de execução longa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a7400a3170b104646607c16852a796d01b64200e
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007146"
---
# <a name="printoperationstatus-complex-type"></a>tipo complexo printOperationStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status atual de uma operação de impressão universal de execução longa.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|state|printOperationProcessingState|O estado de processamento atual da operação. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|description|String|Uma descrição legível do estado de processamento atual da operação. Somente leitura.|

### <a name="printoperationprocessingstate-values"></a>valores de printOperationProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|notStarted|,0|A operação ainda não foi iniciada.|
|com|1 |A operação está sendo executada.|
|adicionada|2 |A operação foi concluída com êxito.|
|falhou|3 |Falha na operação.|
|unknownFutureValue|4 |Valor de sentinela de enumeração evolvable. Não usar.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printOperationStatus"
}-->

```json
{
    "state": "String",
    "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printOperationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->