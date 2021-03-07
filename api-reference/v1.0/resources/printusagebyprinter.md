---
title: Tipo de recurso printUsageByPrinter
description: Descreve a atividade de impressão de uma impressora durante um período de tempo especificado (usageDate).
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 8c5a69d01f0b8da05a5f72f5c2c7d9bacf10ff1a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517012"
---
# <a name="printusagebyprinter-resource-type"></a>Tipo de recurso printUsageByPrinter

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Descreve a atividade de impressão de uma impressora durante um período de tempo especificado (usageDate).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Lista (diariamente)](../api/reportroot-list-dailyprintusagebyprinter.md) | [printUsageByPrinter](printUsageByPrinter.md) | Obter uma lista de resumos de uso diário de impressão, agrupados por impressora. |
| [Lista (mensal)](../api/reportroot-list-monthlyprintusagebyprinter.md) | [printUsageByPrinter](printUsageByPrinter.md) | Obter uma lista de resumos de uso de impressão mensal, agrupados por impressora. |
| [Get](../api/printUsageByPrinter-get.md) | [printUsageByPrinter](printUsageByPrinter.md) | Leia as propriedades e as relações de um **objeto printUsageByPrinter.** |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
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
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUsageByPrinter",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUsageByPrinter",
  "id": "String (identifier)",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "printerId": "String"
}
```

