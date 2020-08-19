---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32c271e7d977ee580974ed5f436a5fc65c38d371
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806398"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageCatalog = new AccessPackageCatalog
{
    DisplayName = "Catalog One"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{accessPackageCatalogId}"]
    .Request()
    .UpdateAsync(accessPackageCatalog);

```