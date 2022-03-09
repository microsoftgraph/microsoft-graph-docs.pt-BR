---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87de834f946c9589232e7a3f5799242124690500
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397705"
---
```powershell

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

$params = @{
    MessageIds = @(
        "MC172851"
        "MC167983"
    )
}

Invoke-MgMarkServiceAnnouncementMessageRead -BodyParameter $params

```