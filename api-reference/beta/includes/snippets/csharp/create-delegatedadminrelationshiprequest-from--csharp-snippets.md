---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47908dffc39e443719603a4cf48b234285f4c3e7
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203455"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedAdminRelationshipRequest = new DelegatedAdminRelationshipRequestObject
{
    Action = DelegatedAdminRelationshipRequestAction.LockForApproval
};

await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"].Requests
    .Request()
    .AddAsync(delegatedAdminRelationshipRequest);

```