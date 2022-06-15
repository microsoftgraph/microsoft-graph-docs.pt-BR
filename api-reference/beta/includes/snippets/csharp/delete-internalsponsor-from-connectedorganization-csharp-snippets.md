---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09fa3a72bee1207707e2035fa8c2a9ab591cfe3fabec92d593d4979aae137e31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100532"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganization-id}"].InternalSponsors["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```