---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8be21535984358f9ec66f870b05f54dc17552ee
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Teamwork.InstalledApps["{userScopeTeamsAppInstallation-id}"]
    .Request()
    .DeleteAsync();

```