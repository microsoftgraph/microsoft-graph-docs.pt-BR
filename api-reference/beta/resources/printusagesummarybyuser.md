---
title: Tipo de recurso printUsageSummaryByUser
description: Descreve a atividade de impressão de um usuário durante um período de tempo especificado (usageDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bba9f57799a36bef4a90b7c514a5be4b4846565e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753579"
---
# <a name="printusagesummarybyuser-resource-type"></a>Tipo de recurso printUsageSummaryByUser

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve a atividade de impressão de um usuário durante um período de tempo especificado (usageDate).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Lista (diariamente)](../api/reportroot-list-dailyprintusagesummariesbyuser.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | Obter uma lista de resumos de uso diário de impressão, agrupados por usuário. |
| [Lista (mensal)](../api/reportroot-list-monthlyprintusagesummariesbyuser.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | Obter uma lista de resumos de uso de impressão mensal, agrupados por usuário. |
| [Get](../api/printusagesummarybyuser-get.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | Ler propriedades e relações de um objeto printUsageSummaryByUser. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|A ID deste resumo de uso.|
|userPrincipalName|Cadeia de caracteres|O UPN do usuário representado por essas estatísticas.|
|usageDate|Data|A data associada a essas estatísticas.|
|completedBlackAndWhiteJobCount|Int64|O número de trabalhos de impressão em preto e branco concluídos em nome do usuário na data associada.|
|completedColorJobCount|Int64|O número de trabalhos de impressão de cores concluídos em nome do usuário na data associada.|
|incompleteJobCount|Int64|O número de trabalhos de impressão que foram enraizadas em nome do usuário, mas não concluídos, na data associada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByUser"
}-->

```json
{
    "id": "String (identifier)",
    "userPrincipalName": "String (identifier)",
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
  "description": "printUsageSummaryByUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

