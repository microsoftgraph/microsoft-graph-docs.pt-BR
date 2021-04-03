---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff18513bd5f9f4a0095f1cd7e7fd4e427f71a905
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("9028d19c-26a9-4809-8e3f-20ff73e2d75e"),
    ResourceId = Guid.Parse("8fce32da-1246-437b-99cd-76d1d4677bd5"),
    AppRoleId = Guid.Parse("498476ce-e0fe-48b0-b801-37ba7e2685c6")
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```