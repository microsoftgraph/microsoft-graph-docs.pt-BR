---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8d4c869885304c6c061a44311ef1de8dd97952b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337936"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AssignmentRequests["{accessPackageAssignmentRequest-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```