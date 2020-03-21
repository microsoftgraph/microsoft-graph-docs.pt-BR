---
title: tipo de recurso archivedPrintJob
description: Um registro de um trabalho de impressão "estado final" (concluído, anulado ou com falha) que é usado para fins de relatório. Este não é um trabalho de impressão ativo.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 170f3b735b4f14173058efbaaa1c81b80490f020
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895474"
---
# <a name="archivedprintjob-resource-type"></a>tipo de recurso archivedPrintJob

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um registro de um trabalho de impressão "estado final" (concluído, anulado ou com falha) que é usado para fins de relatório. Este não é um trabalho de impressão ativo.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O GUID do trabalho de impressão arquivado. Somente leitura.|
|printerid|String|A ID da impressora para a qual o trabalho foi enfileirado. Somente leitura.|
|ProcessingState|printJobProcessingState|O estado de processamento final do trabalho de impressão. Somente leitura.|
|createdDateTime|DateTimeOffset|O dateTimeOffset quando o trabalho foi criado. Somente leitura.|
|acquiredDateTime|DateTimeOffset|O dateTimeOffset quando o trabalho foi adquirido pela impressora, se houver. Somente leitura.|
|completionDateTime|DateTimeOffset|O dateTimeOffset quando o trabalho foi concluído, cancelado ou anulado. Somente leitura.|
|acquiredByPrinter|Boolean|True se o trabalho foi adquirido por uma impressora; caso contrário, false. Somente leitura.|
|copiesPrinted|Int32|O número de cópias que foram impressas. Somente leitura.|
|pageCount|Int32|O número total de páginas que foram impressas. Somente leitura.|
|blackAndWhitePageCount|Int32|O número de páginas em preto e branco que foram impressas. Somente leitura.|
|colorPageCount|Int32|O número de páginas de cores que foram impressas. Somente leitura.|
|simplexPageCount|Int32|O número de páginas simplex (de lado único) que foram impressas. Somente leitura.|
|duplexPageCount|Int32|O número de páginas duplex (frente e verso) que foram impressas. Somente leitura.|
|createdBy|[userIdentity](useridentity.md)|O usuário que criou o trabalho de impressão. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.archivedPrintJob"
}-->

```json
{
    "id": "String (identifier)",
    "printer": {"@odata.type": "microsoft.graph.directoryObject"},
    "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
    "processingState": {"@odata.type": "microsoft.graph.printJobProcessingState"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "archivedPrintJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->