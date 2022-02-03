---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 859bb73c4fc41ea84847995add65ddd69deaaf36
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349637"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Name = "Personal events"
}

# A UPN can also be used as -UserId.
New-MgUserCalendarGroup -UserId $userId -BodyParameter $params

```