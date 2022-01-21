---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d9d057c36d70aefd99676abae66494fa0727392
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131078"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    "@odata.type" = "#microsoft.graph.linkedResource"
    WebUrl = "http://microsoft.com"
    ApplicationName = "Microsoft"
    DisplayName = "Microsoft"
}

Update-MgUserTodoListTaskLinkedResource -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -LinkedResourceId $linkedResourceId -BodyParameter $params

```