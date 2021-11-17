---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1354e543678bd3264ee79d3bac77e6706847c1f586f6e851a8c586a90db75b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898805"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies["{accessPackageAssignmentPolicy-id}"]
    .Request()
    .DeleteAsync();

```