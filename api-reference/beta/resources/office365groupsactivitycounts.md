---
title: tipo de recurso office365GroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 6c67de6592d32c15e7d64112ce9ac31b6a5d4c41
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092423"
---
# <a name="office365groupsactivitycounts-resource-type"></a>tipo de recurso office365GroupsActivityCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo   | Descrição                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | Data   | A última data do conteúdo.          |
| exchangeEmailsReceived | Int64  | O número de emails recebidos por caixas de correio de grupo. |
| yammerMessagesPosted   | Int64  | O número de mensagens postadas nos grupos do Yammer. |
| yammerMessagesRead     | Int64  | O número de mensagens lidas nos grupos do Yammer. |
| yammerMessagesLiked    | Int64  | O número de mensagens curtidas em grupos do Yammer. |
| reportDate             | Data   | A data em que um número de emails foi enviado para uma caixa de correio de grupo ou várias mensagens foram postadas, lidas ou curtidas em um grupo do Yammer |
| reportPeriod           | Cadeia de caracteres | O número de dias que o relatório cobre.    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeEmailsReceived": 1024, 
  "yammerMessagesPosted": 1024, 
  "yammerMessagesRead": 1024, 
  "yammerMessagesLiked": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


