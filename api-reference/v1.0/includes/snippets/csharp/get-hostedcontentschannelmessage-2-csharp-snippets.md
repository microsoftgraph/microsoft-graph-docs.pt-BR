---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b966b335a44436ba2b4015cdd38ac032b7a50d8d086dc1b8714335cbc24316b7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326921"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hostedContents = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"].Replies["{chatMessage-id}"].HostedContents
    .Request()
    .GetAsync();

```