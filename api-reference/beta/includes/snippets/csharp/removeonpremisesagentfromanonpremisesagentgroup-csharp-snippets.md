---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff9cb4dcd4794a276af1630900b98805c773969a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878646"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.OnPremisesPublishingProfiles["provisioning"].Agents["1234b780-965f-4149-85c5-a8c73e58b67d"].AgentGroups["8832388F-3814-4952-B288-FFB62081FE25"].Reference
    .Request()
    .DeleteAsync();

```