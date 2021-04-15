---
title: Tipo de recurso teamsUserActivityDistributionUserCounts
description: Representa o número de usuários por tipo de atividade durante o período de tempo selecionado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3d4fa8b3aec98a03d7e51819db0dc4797367f499
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766905"
---
# <a name="teamsuseractivitydistributionusercounts-resource-type"></a>Tipo de recurso teamsUserActivityDistributionUserCounts

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o número de usuários por tipo de atividade durante o período de tempo selecionado.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo   | Descrição                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| reportRefreshDate   | Data   | A data mais recente do conteúdo.                              |
| teamChatMessages    | Int64  | O número de mensagens exclusivas que os usuários postaram em um chat de equipe. |
| privateChatMessages | Int64  | O número de mensagens exclusivas que os usuários postaram em um chat privado. |
| calls               | Int64  | O número de chamadas exclusivas de 1:1 que os usuários participaram.   |
| meetings            | Int64  | O número de reuniões online exclusivas que os usuários participaram. |
| reportPeriod        | String | O número de dias que o relatório aborda.                        |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```


