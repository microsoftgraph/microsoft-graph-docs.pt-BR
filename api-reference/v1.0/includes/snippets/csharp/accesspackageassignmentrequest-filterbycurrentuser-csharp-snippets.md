---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2b79b30be1b9fe6c499fc4f175de6ff67ec2915b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337138"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.EntitlementManagement.AssignmentRequests
    .FilterByCurrentUser(AccessPackageAssignmentRequestFilterByCurrentUserOptions.Target)
    .Request()
    .GetAsync();

```