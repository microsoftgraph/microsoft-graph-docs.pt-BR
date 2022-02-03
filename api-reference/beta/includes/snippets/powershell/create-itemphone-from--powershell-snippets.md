---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecd26fd823b85da64a40c0c55a56d193c405b3c4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351656"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    DisplayName = "Car Phone"
    Number = "+7 499 342 22 13"
}

# A UPN can also be used as -UserId.
New-MgUserProfilePhone -UserId $userId -BodyParameter $params

```