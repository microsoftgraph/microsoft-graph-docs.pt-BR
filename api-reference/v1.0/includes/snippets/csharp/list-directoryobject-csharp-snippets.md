---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aea1094e0559fb4bffc5bc8381fc6a8b75edb93e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335241"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalSponsors = await graphClient.IdentityGovernance.EntitlementManagement.Assignments["{accessPackageAssignment-id}"].Target.ConnectedOrganization.ExternalSponsors
    .Request()
    .GetAsync();

```