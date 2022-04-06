---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3ac4312230e010bd0ffc8f7a9f37d47d16d025a
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63515793"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentApprovals
    .FilterByCurrentUser(ApprovalFilterByCurrentUserOptions.Approver)
    .Request()
    .GetAsync();

```