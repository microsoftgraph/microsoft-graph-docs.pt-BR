---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18e7d31acca1617a6a53e06e0324179b3467901a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122698"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    PrincipalId = "cde330e5-2150-4c11-9c5b-14bfdc948c79"
    ResourceId = "8e881353-1735-45af-af21-ee1344582a4d"
    AppRoleId = "00000000-0000-0000-0000-000000000000"
}

New-MgUserAppRoleAssignment -UserId $userId -BodyParameter $params

```