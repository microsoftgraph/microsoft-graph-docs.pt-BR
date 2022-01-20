---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: febaf5b0f36f07d05f5438f3dee8b94479c017e1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136657"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Definition = @(
        "definition-value"
    )
    DisplayName = "displayName-value"
    IsOrganizationDefault = $true
}

New-MgPolicyActivityBasedTimeoutPolicy -BodyParameter $params

```