---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7e5add9177c3430b10217f8859eda3b2f3699090507bba537f99a99f5e27913
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hostedContents = await graphClient.Chats["{chat-id}"].Messages["{chatMessage-id}"].HostedContents
    .Request()
    .GetAsync();

```