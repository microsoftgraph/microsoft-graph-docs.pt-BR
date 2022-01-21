---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bad3bd35c32bf47b1bf7cd338793eeeaf6e44326
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131147"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    IsEnabled = $false
}

Update-MgPolicyIdentitySecurityDefaultEnforcementPolicy -BodyParameter $params

```