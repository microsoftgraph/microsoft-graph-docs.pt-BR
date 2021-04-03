---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57e1dc42824eb5bb69c477b02b4398940972d447
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51572983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("cde330e5-2150-4c11-9c5b-14bfdc948c79"),
    ResourceId = Guid.Parse("8e881353-1735-45af-af21-ee1344582a4d"),
    AppRoleId = Guid.Parse("00000000-0000-0000-0000-000000000000")
};

await graphClient.Users["{user-id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```