---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62aeed1f337b7cf035ab717376add691229739b9
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810213"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalSponsors = await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{id}"].ExternalSponsors
    .Request()
    .GetAsync();

```