---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cccc5041e4860991e0657043e0780195b0fb171f
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610354"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hostedContents = await graphClient.Chats["{chat-id}"].Messages["{chatMessage-id}"].HostedContents
    .Request()
    .GetAsync();

```