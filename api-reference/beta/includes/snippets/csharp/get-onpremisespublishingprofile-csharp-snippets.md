---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1c377b0178178ba9744875c6761fbf77bd1d57d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351099"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesPublishingProfile = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"]
    .Request()
    .Expand("publishedResources,agents,agentGroups")
    .GetAsync();

```