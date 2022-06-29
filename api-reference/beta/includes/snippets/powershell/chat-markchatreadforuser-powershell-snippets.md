---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9fc39016f90100168bb62e18ba46ba534615025e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66503118"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    User = @{
        Id = "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
    }
    TenantId = "2a690434-97d9-4eed-83a6-f5f13600199a"
}

Invoke-MgMarkChatReadForUser -ChatId $chatId -BodyParameter $params

```