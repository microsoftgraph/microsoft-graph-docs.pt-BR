---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3987d92b39921ab9bfa4b2b62e78f06967c798eac905b9523696d05e35f11ca0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216830"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userScopeTeamsAppInstallation = await graphClient.Users["{user-id}"].Teamwork.InstalledApps["{userScopeTeamsAppInstallation-id}"]
    .Request()
    .GetAsync();

```