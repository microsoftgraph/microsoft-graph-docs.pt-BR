---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac170e65e875ad517bbb39e2598e0d7303f75fae6e8e7cfe953943c9e619aba6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57330073"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"].Replies["{chatMessage-id}"]
    .Request()
    .GetAsync();

```