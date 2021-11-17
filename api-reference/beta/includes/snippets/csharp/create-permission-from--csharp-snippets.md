---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94c0b4491be13dfd1c407728728886b26c926574c3b4565448877469798a7afc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215145"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permission = new Permission
{
    Roles = new List<String>()
    {
        "write"
    },
    GrantedToIdentities = new List<IdentitySet>()
    {
        new IdentitySet
        {
            Application = new Identity
            {
                Id = "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
                DisplayName = "Contoso Time Manager App"
            }
        }
    }
};

await graphClient.Sites["{site-id}"].Permissions
    .Request()
    .AddAsync(permission);

```