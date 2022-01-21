---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e60ed3cb03c8ba84548023520573b7a949baefcc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129843"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    RequestType = "AdminRemove"
    AccessPackageAssignment = @{
        Id = "a6bb6942-3ae1-4259-9908-0133aaee9377"
    }
}

New-MgEntitlementManagementAccessPackageAssignmentRequest -BodyParameter $params

```