---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5b1d7037a144a9982443b527e44791287a0eca0f
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946761"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Title = "A new task"
    Categories = @(
        "Important"
    )
    LinkedResources = @(
        @{
            WebUrl = "http://microsoft.com"
            ApplicationName = "Microsoft"
            DisplayName = "Microsoft"
        }
    )
}

# A UPN can also be used as -UserId.
New-MgUserTodoListTask -UserId $userId -TodoTaskListId $todoTaskListId -BodyParameter $params

```