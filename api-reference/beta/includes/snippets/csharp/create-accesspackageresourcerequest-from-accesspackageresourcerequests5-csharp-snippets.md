---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 969eca93c95cc91efa48c98d263413004329ee827618cc9d89c5ac0ac8245592
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156578"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRequest = new AccessPackageResourceRequestObject
{
    CatalogId = "beedadfe-01d5-4025-910b-84abb9369997",
    RequestType = "AdminRemove",
    AccessPackageResource = new AccessPackageResource
    {
        Id = "354078e5-dbce-4894-8af4-0ab274d41662"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceRequests
    .Request()
    .AddAsync(accessPackageResourceRequest);

```