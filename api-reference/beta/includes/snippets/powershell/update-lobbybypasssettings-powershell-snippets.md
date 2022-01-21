---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86be61b9b033446d00525df63b34aaef0752107f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133345"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    LobbyBypassSettings = @{
        IsDialInBypassEnabled = $true
    }
}

Update-MgUserOnlineMeeting -UserId $userId -OnlineMeetingId $onlineMeetingId -BodyParameter $params

```