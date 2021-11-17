---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6798b423c66774d82d82c10a51fb55f40a63ca84f8ee80edf6bf594e0b3c18fd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326724"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agentGroups = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].AgentGroups
    .Request()
    .Expand("publishedResources")
    .GetAsync();

```