---
title: tipo de recurso office365GroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: f07743a592753daff2670478c6f2fe18207f6013
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522453"
---
# <a name="office365groupsactivitycounts-resource-type"></a>tipo de recurso office365GroupsActivityCounts

Namespace: Microsoft. Graph

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo   | Descrição                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | Data   | A última data do conteúdo.          |
| exchangeEmailsReceived | Int64  | O número de emails recebidos por caixas de correio de grupo. |
| yammerMessagesPosted   | Int64  | O número de mensagens postadas nos grupos do Yammer. |
| yammerMessagesRead     | Int64  | O número de mensagens lidas nos grupos do Yammer. |
| yammerMessagesLiked    | Int64  | O número de mensagens curtidas em grupos do Yammer. |
| reportDate             | Data   | A data em que um número de emails foi enviado para uma caixa de correio de grupo ou várias mensagens foram postadas, lidas ou curtidas em um grupo do Yammer |
| reportPeriod           | String | O número de dias que o relatório cobre.    |

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
