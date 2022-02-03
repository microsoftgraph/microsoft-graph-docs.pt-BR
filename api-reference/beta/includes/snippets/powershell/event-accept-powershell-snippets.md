---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d762dad8c628c60fb1770b4fde1ef5bf1f2a6e2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343197"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Comment = "comment-value"
    SendResponse = $true
}

# A UPN can also be used as -UserId.
Invoke-MgAcceptUserEvent -UserId $userId -EventId $eventId -BodyParameter $params

```