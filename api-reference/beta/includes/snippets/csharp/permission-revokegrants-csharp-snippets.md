---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56beab12fcdf30833d9e23c91b869af4d14c2749
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778048"
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

await graphClient.Me.Drive.Items["{driveItem-id}"].Permissions["{permission-id}"]
    .RevokeGrants(grantees)
    .Request()
    .PostAsync();

```