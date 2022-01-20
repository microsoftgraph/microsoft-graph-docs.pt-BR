---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2e6025e185af9faf9766d857e89aad5aecf48323
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109172"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Id = "c1"
    DisplayName = "Contoso medium"
    Description = "Medium protection level defined for Contoso policy"
    IsAvailable = $true
}

New-MgIdentityConditionalAccessAuthenticationContextClassReference -BodyParameter $params

```