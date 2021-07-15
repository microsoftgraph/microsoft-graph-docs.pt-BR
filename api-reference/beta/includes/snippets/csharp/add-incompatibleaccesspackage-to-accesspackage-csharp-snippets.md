---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 868de6474c0b0d432f3de71a7ace07e7d92862f9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439831"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackage = new AccessPackage
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2"}
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].IncompatibleAccessPackages.References
    .Request()
    .AddAsync(accessPackage);

```