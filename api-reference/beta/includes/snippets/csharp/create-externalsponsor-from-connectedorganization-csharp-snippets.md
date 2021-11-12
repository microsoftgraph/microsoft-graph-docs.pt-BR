---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3adba746ab0a76610dd31498f4e449307a90057cb67156abbfdf1bfdbb3802d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganization-id}"].ExternalSponsors.References
    .Request()
    .AddAsync(directoryObject);

```