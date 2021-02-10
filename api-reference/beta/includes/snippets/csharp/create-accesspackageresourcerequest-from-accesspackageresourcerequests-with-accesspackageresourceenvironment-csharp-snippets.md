---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2bf2874e1b0bd883d278ea72bfadaa3eafa16dd3
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176327"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRequest = new AccessPackageResourceRequestObject
{
    CatalogId = "de9315c1-272b-4905-924b-cc112ca180c7",
    AccessPackageResource = new AccessPackageResource
    {
        DisplayName = "Community Outreach",
        Description = "https://contoso.sharepoint.com/sites/CSR",
        ResourceType = "SharePoint Online Site",
        OriginId = "https://contoso.sharepoint.com/sites/CSR",
        OriginSystem = "SharePointOnline",
        AdditionalData = new Dictionary<string, object>()
        {
            {"accessPackageResourceEnvironment@odata.bind", "accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57"}
        }
    },
    RequestType = "AdminAdd"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceRequests
    .Request()
    .AddAsync(accessPackageResourceRequest);

```