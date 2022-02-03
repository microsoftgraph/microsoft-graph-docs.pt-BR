---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7f40a75ff2fc03b848ca4b1e4e4a1d0fef834abb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352594"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Name = "Volunteer"
}

# A UPN can also be used as -UserId.
New-MgUserCalendar -UserId $userId -BodyParameter $params

```