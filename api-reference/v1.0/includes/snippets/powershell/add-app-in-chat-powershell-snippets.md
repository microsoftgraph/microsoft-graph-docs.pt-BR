---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 901cd13fb2679cc2aa6a2c81ee3bc353bada9a89
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122300"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "TeamsApp@odata.bind" = "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}

New-MgChatInstalledApp -ChatId $chatId -BodyParameter $params

```