---
title: Tipo de recurso printUsageSummaryByPrinter
description: Descreve a atividade de impressão de uma impressora durante um período de tempo especificado (usageDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4d33ab99780f980dcc24e267ba1ac6603f602aa2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753580"
---
# <a name="printusagesummarybyprinter-resource-type"></a>Tipo de recurso printUsageSummaryByPrinter

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve a atividade de impressão de uma impressora durante um período de tempo especificado (usageDate).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Lista (diariamente)](../api/reportroot-list-dailyprintusagesummariesbyprinter.md) | [printUsageSummaryByPrinter](printusagesummarybyprinter.md) | Obter uma lista de resumos de uso diário de impressão, agrupados por impressora. |
| [Lista (mensal)](../api/reportroot-list-monthlyprintusagesummariesbyprinter.md) | [printUsageSummaryByPrinter](printusagesummarybyprinter.md) | Obter uma lista de resumos de uso de impressão mensal, agrupados por impressora. |
| [Get](../api/printusagesummarybyprinter-get.md) | [printUsageSummaryByPrinter](printusagesummarybyprinter.md) | Leia as propriedades e as relações de um **objeto printUsageSummaryByPrinter.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|A ID deste resumo de uso.|
|printerID|Cadeia de caracteres|A ID da impressora representada por essas estatísticas.|
|usageDate|Data|A data associada a essas estatísticas.|
|completedBlackAndWhiteJobCount|Int64|O número de trabalhos de impressão em preto e branco concluídos pela impressora na data associada.|
|completedColorJobCount|Int64|O número de trabalhos de impressão de cores concluídos pela impressora na data associada.|
|incompleteJobCount|Int64|O número de trabalhos de impressão que foram enraizadas para a impressora, mas não concluídos, na data associada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter"
}-->

```json
{
    "id": "String (identifier)",
    "printerId": "String (identifier)",
    "usageDate": "String (timestamp)",
    "completedBlackAndWhiteJobCount": 123456,
    "completedColorJobCount": 123456,
    "incompleteJobCount": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUsageSummaryByPrinter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

