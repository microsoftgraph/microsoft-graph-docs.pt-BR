---
title: Tipo de recurso office365GroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: a212028e4ba9d38ea38e99c835d89fe1fe7d850b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980693"
---
# <a name="office365groupsactivitycounts-resource-type"></a>Tipo de recurso office365GroupsActivityCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo   | Descrição                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | Data   | A data mais recente do conteúdo.          |
| exchangeEmailsReceived | Int64  | O número de emails recebidos pelas caixas de correio de Grupo. |
| yammerMessagesPosted   | Int64  | O número de mensagens postadas em grupos do Yammer. |
| yammerMessagesRead     | Int64  | O número de mensagens lidas em grupos do Yammer. |
| yammerMessagesLiked    | Int64  | O número de mensagens curtidas em grupos do Yammer. |
| reportDate             | Data   | A data em que vários emails foram enviados para uma caixa de correio de grupo ou várias mensagens postadas, lidas ou curtidas em um grupo do Yammer |
| reportPeriod           | Cadeia de caracteres | O número de dias que o relatório abrange.    |

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


