---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca7595058bcaa86ae799d1046b3fad3823861169
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337240"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["{team-id}"].InstalledApps
    .Request()
    .Filter("teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .Expand("teamsApp,teamsAppDefinition")
    .GetAsync();

```