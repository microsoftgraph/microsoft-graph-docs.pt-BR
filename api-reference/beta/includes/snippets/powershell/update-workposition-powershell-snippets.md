---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce9643af7f90613eaf0241fdc133b72a8016ab2f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349990"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    IsCurrent = $true
}

# A UPN can also be used as -UserId.
Update-MgUserProfilePosition -UserId $userId -WorkPositionId $workPositionId -BodyParameter $params

```