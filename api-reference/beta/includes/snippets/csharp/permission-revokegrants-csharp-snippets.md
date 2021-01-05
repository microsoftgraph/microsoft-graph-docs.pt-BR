---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee692b40e410bc3f15752d679bf802fbaa232655
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753159"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var grantees = new List<DriveRecipient>()
{
    new DriveRecipient
    {
        Email = "ryan@contoso.com"
    }
};

await graphClient.Me.Drive.Items["{item-id}"].Permissions["{perm-id}"]
    .RevokeGrants(grantees)
    .Request()
    .PostAsync();

```