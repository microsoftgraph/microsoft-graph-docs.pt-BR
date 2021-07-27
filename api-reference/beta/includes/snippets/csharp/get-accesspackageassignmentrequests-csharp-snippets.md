---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1cf9d3fe25656a849302bbcfbe81cfff91f3057
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581652"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequests = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests
    .Request()
    .Filter("(requestState eq 'PendingApproval')")
    .Expand("requestor($expand=connectedOrganization)")
    .GetAsync();

```