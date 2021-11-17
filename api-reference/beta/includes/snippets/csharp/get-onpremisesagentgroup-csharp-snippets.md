---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5dbcbcaf74ca9a943be623314c666a6c38a2f142ad78a19433343fc6df1193d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160084"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesAgentGroup = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].AgentGroups["{onPremisesAgentGroup-id}"]
    .Request()
    .Expand("agents")
    .GetAsync();

```