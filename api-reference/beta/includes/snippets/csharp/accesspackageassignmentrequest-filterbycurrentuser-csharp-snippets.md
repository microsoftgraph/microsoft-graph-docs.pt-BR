---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b2235628482180fabf6edcbd9c7c467f00e3a09c518e22b872157bcbcd9212b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898785"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages
    .FilterByCurrentUser(AccessPackageFilterByCurrentUserOptions.AllowedRequestor)
    .Request()
    .GetAsync();

```