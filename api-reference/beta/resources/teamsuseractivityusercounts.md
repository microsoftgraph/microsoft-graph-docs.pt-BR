---
title: Tipo de recurso teamsUserActivityUserCounts
description: Representa números de usuários diários por tipo de atividade.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f1ddb3e6e5e6a0b6fbb5c9973bec7e29f4492089
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766438"
---
# <a name="teamsuseractivityusercounts-resource-type"></a>Tipo de recurso teamsUserActivityUserCounts

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa números de usuários diários por tipo de atividade.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo   | Descrição                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| reportRefreshDate   | Data   | A data mais recente do conteúdo.                              |
| reportDate          | Data   | A data em que os usuários realizaram as atividades.        |
| teamChatMessages    | Int64  | O número de usuários que postaram mensagens em um chat de equipe.       |
| privateChatMessages | Int64  | O número de usuários que postaram mensagens em um chat privado.    |
| calls               | Int64  | O número de usuários que participaram de chamadas 1:1.           |
| meetings            | Int64  | O número de usuários que participaram de reuniões online.     |
| otherActions        | Int64  | O número de usuários que estavam ativos, mas realizaram outras atividades que não os tipos de ação expostos oferecidos no relatório (enviando ou respondendo a mensagens de canal e mensagens de chat, agendando ou participando de chamadas e reuniões 1:1). Exemplos de ações são quando um usuário altera o status do Teams ou a mensagem de status do Teams ou abre uma postagem mensagem de canal, mas não responde. |
| reportPeriod        | String | O número de dias que o relatório aborda.                        |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```


