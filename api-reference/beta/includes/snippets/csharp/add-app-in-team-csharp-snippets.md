---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 373e15eb48dcae40b03689900d1311cdd3f1a989
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690310"
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

await graphClient.Teams["87654321-0abc-zqf0-321456789q"].InstalledApps
    .Request()
    .AddAsync(teamsAppInstallation);

```