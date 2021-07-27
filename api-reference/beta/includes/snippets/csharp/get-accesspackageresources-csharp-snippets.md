---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b53fff4b18cff4b1722f97243ef2c0163d2ba0f2
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581123"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResources = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{accessPackageCatalog-id}"].AccessPackageResources
    .Request()
    .Filter("resourceType eq 'Application'")
    .Expand("accessPackageResourceScopes")
    .GetAsync();

```