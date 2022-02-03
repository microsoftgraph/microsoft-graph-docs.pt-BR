---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0f27f87afd78a9c3a0fa9666d16535a8b22220b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346776"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    GroupIds = @(
        "fee2c45b-915a-4a64b130f4eb9e75525e"
        "4fe90ae065a-478b9400e0a0e1cbd540"
    )
}

# A UPN can also be used as -UserId.
Confirm-MgUserMemberGroup -UserId $userId -BodyParameter $params

```