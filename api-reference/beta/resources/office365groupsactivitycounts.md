---
title: Tipo de recurso office365GroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 28ac5ad72a9e0b7e32336b397c0df114abf6fc9b88368f983dd84413ca4fe96e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226137"
---
# <a name="office365groupsactivitycounts-resource-type"></a>Tipo de recurso office365GroupsActivityCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo   | Descrição                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | Data   | A data mais recente do conteúdo.          |
| exchangeEmailsReceived | Int64  | O número de emails recebidos pelas caixas de correio de grupo. |
| yammerMessagesPosted   | Int64  | O número de mensagens postadas em Yammer grupos. |
| yammerMessagesRead     | Int64  | O número de mensagens lidas em Yammer grupos. |
| yammerMessagesLiked    | Int64  | O número de mensagens curtidas em Yammer grupos. |
| reportDate             | Data   | A data em que vários emails foram enviados para uma caixa de correio de grupo ou várias mensagens foram postadas, lidas ou curtidas em um grupo Yammer grupo |
| reportPeriod           | Cadeia de caracteres | O número de dias que o relatório aborda.    |

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


