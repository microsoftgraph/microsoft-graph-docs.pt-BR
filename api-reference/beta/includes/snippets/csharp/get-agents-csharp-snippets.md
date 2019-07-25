---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27237b7467100b49453b35c7f2b76b90560570b6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agents = await graphClient.OnPremisesPublishingProfiles["provisioning"].Agents
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```