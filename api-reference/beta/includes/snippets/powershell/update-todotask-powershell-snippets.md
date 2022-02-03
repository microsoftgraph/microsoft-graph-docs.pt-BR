---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a6dac60fb2f998740bdafa4304f3394daea599b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349957"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DueDateTime = @{
        DateTime = "2020-07-25T16:00:00"
        TimeZone = "Eastern Standard Time"
    }
}

# A UPN can also be used as -UserId.
Update-MgUserTodoListTask -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -BodyParameter $params

```