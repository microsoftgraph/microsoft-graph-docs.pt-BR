---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3353f7f1367c465ed34f532bc13aaddceea699ce
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346703"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectedOrganization = new ConnectedOrganization
{
    DisplayName = "Connected organization new name",
    Description = "Connected organization new description",
    State = ConnectedOrganizationState.Configured
};

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganization-id}"]
    .Request()
    .UpdateAsync(connectedOrganization);

```