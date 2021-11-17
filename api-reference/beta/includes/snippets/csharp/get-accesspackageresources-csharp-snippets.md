---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20b1ebf07ae8d9e762fb32e4d1acec31d77434e3b30e199d843af0b952ec5232
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResources = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{accessPackageCatalog-id}"].AccessPackageResources
    .Request()
    .Filter("resourceType eq 'Application'")
    .Expand("accessPackageResourceScopes")
    .GetAsync();

```