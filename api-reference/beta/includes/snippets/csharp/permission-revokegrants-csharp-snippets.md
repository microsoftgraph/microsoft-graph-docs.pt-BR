---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2db98c03d2317a21c82673c3a41107866e34f44e9eda51ae8a2f667b6246da04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216348"
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