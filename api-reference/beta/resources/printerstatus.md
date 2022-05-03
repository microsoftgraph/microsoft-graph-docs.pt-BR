---
title: Tipo de recurso printerStatus
description: Representa o status de processamento da impressora, incluindo erros.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4b405fe00ab7dfe0e3ce90e79b1e7a82607f012c
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176543"
---
# <a name="printerstatus-resource-type"></a>Tipo de recurso printerStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de processamento da impressora, incluindo erros.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|state|printerProcessingState|O estado de processamento atual. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|detalhes|Coleção printerProcessingStateDetail|A lista de detalhes que descrevem por que a impressora está no estado atual. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|description|Cadeia de caracteres|Uma descrição legível por humanos do estado de processamento atual da impressora. Somente leitura.|

### <a name="printerprocessingstate-values"></a>Valores printerProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|O estado de processamento relatado pela impressora é desconhecido.|
|Ocioso|1|A impressora está ociosa e pronta para aceitar novos trabalhos de impressão.|
|Processamento|2|No momento, a impressora está processando um trabalho de impressão e processará todos os trabalhos pendentes após a conclusão.|
|Parou|3|A impressora encontrou um problema (por exemplo, ficou sem papel na bandeja ativa) e não pode continuar o trabalho de impressão atual até que o problema seja resolvido. Consulte os **valores de** detalhes ou o valor **de descrição** para obter mais informações.|
|unknownFutureValue|4|Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="printerprocessingstatedetail-values"></a>Valores printerProcessingStateDetail

[Tipo de enumeração printerProcessingStateDetail](./printerprocessingstatedetail.md)

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerStatus"
}-->

```json
{
    "state": "String",
    "details": ["String"],
    "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

