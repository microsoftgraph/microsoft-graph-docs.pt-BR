---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1c5c38d654a9012e3978369fcc745b62d0fef0d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tabs = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Tabs
    .Request()
    .Filter("teamsApp/id eq 'com.microsoft.teamspace.tab.planner'")
    .Expand("teamsApp")
    .GetAsync();

```