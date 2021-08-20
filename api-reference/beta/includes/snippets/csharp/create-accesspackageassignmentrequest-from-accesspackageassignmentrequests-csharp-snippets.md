---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 470f79f7aa3d5b05c8121a22188f3ffec237e551bdaf234b09b6c94020860fe9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099853"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = new AccessPackageAssignmentRequestObject
{
    RequestType = "AdminRemove",
    AccessPackageAssignment = new AccessPackageAssignment
    {
        Id = "a6bb6942-3ae1-4259-9908-0133aaee9377"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests
    .Request()
    .AddAsync(accessPackageAssignmentRequest);

```