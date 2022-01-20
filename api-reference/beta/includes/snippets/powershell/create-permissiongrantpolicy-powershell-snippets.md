---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 108a11a34dfab56a76d05ee9fc60ceea248b40db
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112499"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Id = "my-custom-consent-policy"
    DisplayName = "Custom application consent policy"
    Description = "A custom permission grant policy to customize conditions for granting consent."
}

New-MgPolicyPermissionGrantPolicy -BodyParameter $params

```