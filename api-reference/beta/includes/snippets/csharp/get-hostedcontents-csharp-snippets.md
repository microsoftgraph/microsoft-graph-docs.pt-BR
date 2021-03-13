---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cccc5041e4860991e0657043e0780195b0fb171f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780475"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hostedContents = await graphClient.Chats["{chat-id}"].Messages["{chatMessage-id}"].HostedContents
    .Request()
    .GetAsync();

```