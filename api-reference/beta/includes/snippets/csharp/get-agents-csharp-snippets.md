---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9a0278f09f6ba0de37a95a478fcde6da2e83ede99a65c24e805267df6b961a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agents = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Agents
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```