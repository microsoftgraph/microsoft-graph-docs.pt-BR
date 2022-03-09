---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31e64443db3f6913f59c5fa1190d5f9d9b926c65
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63398020"
---
```powershell

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

$params = @{
    MessageIds = @(
        "MC172851"
        "MC167983"
    )
}

Invoke-MgMarkServiceAnnouncementMessageUnread -BodyParameter $params

```