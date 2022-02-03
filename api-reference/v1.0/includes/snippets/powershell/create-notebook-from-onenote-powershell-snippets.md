---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85aa72b961f28d441e2859ee3440821eedd3dae7
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352748"
---
```powershell

Import-Module Microsoft.Graph.Notes

$params = @{
    DisplayName = "My Private notebook"
}

# A UPN can also be used as -UserId.
New-MgUserOnenoteNotebook -UserId $userId -BodyParameter $params

```