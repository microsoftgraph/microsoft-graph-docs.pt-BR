---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ef46868e989f83094938f898254d8e3f02040f1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352242"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Address = "Innocenty.Popov@adventureworks.com"
}

# A UPN can also be used as -UserId.
New-MgUserProfileEmail -UserId $userId -BodyParameter $params

```