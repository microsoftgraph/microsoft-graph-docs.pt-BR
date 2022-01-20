---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4f5a96bd10cdb5dc194530c29357ff6c92691dd2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131563"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "Architecture Discussion"
    Description = "This channel is where we debate all future architecture plans"
    MembershipType = "standard"
}

New-MgTeamChannel -TeamId $teamId -BodyParameter $params

```