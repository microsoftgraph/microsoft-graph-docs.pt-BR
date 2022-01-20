---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: beca6bf63dae4a74245d879234cee204a65247c5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107863"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "TeamsApp@odata.bind" = "https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}

New-MgUserTeamworkInstalledApp -UserId $userId -BodyParameter $params

```