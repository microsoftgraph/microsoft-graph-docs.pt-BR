---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 185abf5379bf9bddc47ae93b14935d67ca95c34d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397830"
---
```powershell

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

$params = @{
    MessageIds = @(
        "MC172851"
        "MC167983"
    )
}

Invoke-MgFavoriteServiceAnnouncementMessage -BodyParameter $params

```