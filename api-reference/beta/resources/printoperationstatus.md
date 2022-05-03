---
title: Tipo de recurso printOperationStatus
description: Representa o status atual de uma operação de Impressão Universal de execução longa.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 79cc94a38335bede616ef57bc33db12db63a5664
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176659"
---
# <a name="printoperationstatus-complex-type"></a>Tipo complexo printOperationStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status atual de uma operação de Impressão Universal de execução longa.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|state|printOperationProcessingState|O estado de processamento atual da printOperation. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|description|Cadeia de caracteres|Uma descrição legível por humanos do estado de processamento atual da printOperation. Somente leitura.|

### <a name="printoperationprocessingstate-values"></a>Valores printOperationProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|Notstarted|0|A operação ainda não foi iniciada.|
|Executando|1|A operação está em execução.|
|Conseguiu|2|A operação foi concluída com êxito.|
|Falhou|3|Falha na operação.|
|unknownFutureValue|4|Valor de sentinel de enumeração evolvável. Não usar.|

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

