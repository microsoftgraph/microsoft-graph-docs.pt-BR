---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef2be2238bf487d1671c476419f58766c5c79d16fe3f5a8d18a77ee42196586f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215361"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Agents["{onPremisesAgent-id}"].AgentGroups["{onPremisesAgentGroup-id}"].Reference
    .Request()
    .DeleteAsync();

```