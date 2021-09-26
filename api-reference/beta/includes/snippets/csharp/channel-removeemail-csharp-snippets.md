---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 873fccbbed33f35bd1890a9131a8936f6e4f184612f5bbbcbab23e5bb34bbcb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898838"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .RemoveEmail()
    .Request()
    .PostAsync();

```