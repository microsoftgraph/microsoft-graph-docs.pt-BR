---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57b4d1665b8295fbacf543d82e310036f249ff22
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132597"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    IsCurrent = $true
}

Update-MgUserProfilePosition -UserId $userId -WorkPositionId $workPositionId -BodyParameter $params

```