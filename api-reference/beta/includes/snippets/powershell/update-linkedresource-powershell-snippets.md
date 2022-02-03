---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1418b2def698804684d6ff945173b44cf0efad3c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351309"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    "@odata.type" = "#microsoft.graph.linkedResource"
    WebUrl = "http://microsoft.com"
    ApplicationName = "Microsoft"
    DisplayName = "Microsoft"
}

# A UPN can also be used as -UserId.
Update-MgUserTodoListTaskLinkedResource -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -LinkedResourceId $linkedResourceId -BodyParameter $params

```