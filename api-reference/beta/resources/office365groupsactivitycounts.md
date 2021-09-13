---
title: Tipo de recurso office365GroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: eed42f5baf9a0130c69f9f8e6c026c9e0082d200
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115118"
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
| reportPeriod           | Cadeia de Caracteres | O número de dias que o relatório aborda.    |

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


