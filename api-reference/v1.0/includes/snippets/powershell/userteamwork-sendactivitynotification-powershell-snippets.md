---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d08868f32a110b6fdb3c1190059af49115930cb2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343506"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Topic = @{
        Source = "entityUrl"
        Value = "https://graph.microsoft.com/v1.0/users/{userId}/teamwork/installedApps/{installationId}"
    }
    ActivityType = "taskCreated"
    PreviewText = @{
        Content = "New Task Created"
    }
    TemplateParameters = @(
        @{
            Name = "taskId"
            Value = "Task 12322"
        }
    )
}

Send-MgUserTeamworkActivityNotification -UserId $userId -BodyParameter $params

```