---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b56d91b1040577357bb73e06cf04cd361b6f8c4c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganization-id}"].ExternalSponsors["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```