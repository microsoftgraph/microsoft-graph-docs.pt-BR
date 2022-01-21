---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5e8b7cd68438b9f5d7d1e34e9333208310d83f67
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122846"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "Finance"
}

Update-MgTeamTag -TeamId $teamId -TeamworkTagId $teamworkTagId -BodyParameter $params

```