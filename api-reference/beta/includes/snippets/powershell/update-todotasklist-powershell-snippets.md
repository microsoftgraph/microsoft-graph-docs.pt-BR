---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26afaa3da11b5986c2ad9bc7ea2f83e4bca401d9
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351914"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DisplayName = "Vacation Plan"
}

# A UPN can also be used as -UserId.
Update-MgUserTodoList -UserId $userId -TodoTaskListId $todoTaskListId -BodyParameter $params

```