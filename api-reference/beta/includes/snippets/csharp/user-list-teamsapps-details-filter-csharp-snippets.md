---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 949e3b6806456f40fd4d6e09d985e0418c687d4a
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Users["97a5a533-833d-494b-b543-c0afe026cb96"].Teamwork.InstalledApps
    .Request()
    .Filter("teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .Expand("teamsAppDefinition")
    .GetAsync();

```