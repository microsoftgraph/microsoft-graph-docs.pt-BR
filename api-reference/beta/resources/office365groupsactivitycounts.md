---
title: tipo de recurso de office365GroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 4f3a5bf02f5f477ebab036fc9afa5d35a8061138
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039928"
---
# <a name="office365groupsactivitycounts-resource-type"></a>tipo de recurso de office365GroupsActivityCounts

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo   | Descrição                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | Data   | A última data do conteúdo.          |
| exchangeEmailsReceived | Int64  | O número de emails recebidos por caixas de correio de grupo. |
| yammerMessagesPosted   | Int64  | O número de mensagens postadas em grupos de Yammer. |
| yammerMessagesRead     | Int64  | O número de mensagens lidas em grupos do Yammer. |
| yammerMessagesLiked    | Int64  | O número de mensagens curtidas em grupos do Yammer. |
| reportDate             | Data   | A data em que um número de emails que foram enviado para uma caixa de correio de grupo ou um número de mensagens publicado, ler ou curtidas em um grupo do Yammer |
| reportPeriod           | String | O número de dias que abrange o relatório.    |

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
