---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0187cdd3f7472c84268d82507bda8ddc0102fdf8
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691301"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Users["{id}"].Teamwork.InstalledApps
    .Request()
    .Expand("teamsAppDefinition")
    .GetAsync();

```