---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: caf5a1438e6bc9ffc8eb00da108732c5b4ba96e9
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48317947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectedOrganization = new ConnectedOrganization
{
    DisplayName = "Connected organization new name",
    Description = "Connected organization new description",
    State = ConnectedOrganizationState.Configured
};

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{id}"]
    .Request()
    .UpdateAsync(connectedOrganization);

```