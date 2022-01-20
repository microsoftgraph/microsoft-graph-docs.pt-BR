---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac26e8b1126a4008dc5b6a794f4f28320f788d44
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133492"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    GroupLifetimeInDays = 180
    ManagedGroupTypes = "Selected"
    AlternateNotificationEmails = "admin@contoso.com"
}

Update-MgGroupLifecyclePolicy -GroupLifecyclePolicyId $groupLifecyclePolicyId -BodyParameter $params

```