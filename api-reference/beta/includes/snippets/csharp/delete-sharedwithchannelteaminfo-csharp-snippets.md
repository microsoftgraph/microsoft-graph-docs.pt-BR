---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa4911ad93823b2839f369d655e14faed7928d89
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209241"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].IncomingChannels["{channel-id}"].Reference
    .Request()
    .DeleteAsync();

```