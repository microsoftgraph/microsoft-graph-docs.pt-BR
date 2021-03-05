---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e0dd014d5f27a75f96bc5b52e1916b6619c15d30
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50474981"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Users["{id}"].Teamwork.InstalledApps
    .Request()
    .Expand("teamsAppDefinition($expand=bot)")
    .GetAsync();

```