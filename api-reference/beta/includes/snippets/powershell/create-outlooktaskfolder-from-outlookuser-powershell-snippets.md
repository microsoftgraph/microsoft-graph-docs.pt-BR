---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 264925466b53eaad6d40b792945afbf53158031d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349668"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Name = "Volunteer"
}

# A UPN can also be used as -UserId.
New-MgUserOutlookTaskFolder -UserId $userId -BodyParameter $params

```