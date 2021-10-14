---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2d677fb2f8cb0eef58937ba85aadd86339c2cc3054c6e51fe53164b8050a48d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101490"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = new TeamsAppInstallation
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"teamsApp@odata.bind", "https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"}
    }
};

await graphClient.Teams["{team-id}"].InstalledApps
    .Request()
    .AddAsync(teamsAppInstallation);

```