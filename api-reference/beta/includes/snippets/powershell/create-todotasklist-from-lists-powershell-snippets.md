---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84a4a337e2dbd1633679937cd7e773a1823f52fa
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352174"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DisplayName = "Travel items"
}

# A UPN can also be used as -UserId.
New-MgUserTodoList -UserId $userId -BodyParameter $params

```