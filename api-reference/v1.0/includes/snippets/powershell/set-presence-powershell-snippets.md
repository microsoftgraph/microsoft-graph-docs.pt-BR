---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f9be2c9370481943daef2106e778cb53c84cb47
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340774"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    SessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87"
    Availability = "Available"
    Activity = "Available"
    ExpirationDuration = "PT1H"
}

Set-MgUserPresence -UserId $userId -BodyParameter $params

```