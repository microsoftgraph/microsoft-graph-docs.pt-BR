---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58f862707635d086fc8204cd66cf63509229ae18
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351366"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    WebUrl = "https://microsoft.com"
    ApplicationName = "Microsoft"
    DisplayName = "Microsoft"
    ExternalId = "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}

# A UPN can also be used as -UserId.
New-MgUserTodoListTaskLinkedResource -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -BodyParameter $params

```