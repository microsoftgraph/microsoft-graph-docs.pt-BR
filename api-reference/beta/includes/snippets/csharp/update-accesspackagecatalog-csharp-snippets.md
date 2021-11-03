---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4995ae6a25814c67d1d9a1952f2a937bcdbbe6bfb4bf2629e9bc76bf2d75f28e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageCatalog = new AccessPackageCatalog
{
    DisplayName = "Catalog One"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{accessPackageCatalog-id}"]
    .Request()
    .UpdateAsync(accessPackageCatalog);

```