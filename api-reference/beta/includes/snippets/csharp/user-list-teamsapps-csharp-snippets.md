---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 416c62554b3a800a896450c44ca1e8d1064352ff
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944845"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userScopeTeamsAppInstallation = await graphClient.Users["{id}"].Teamwork.InstalledApps["{id}"]
    .Request()
    .GetAsync();

```