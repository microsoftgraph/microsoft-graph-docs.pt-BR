---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e616ad684ee19a34490cc7e8a12cacfd119cccc8584c7822b05d6033bd34ca1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099533"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesAgentGroup = new OnPremisesAgentGroup
{
    DisplayName = "Group New Name"
};

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].AgentGroups["{onPremisesAgentGroup-id}"]
    .Request()
    .UpdateAsync(onPremisesAgentGroup);

```