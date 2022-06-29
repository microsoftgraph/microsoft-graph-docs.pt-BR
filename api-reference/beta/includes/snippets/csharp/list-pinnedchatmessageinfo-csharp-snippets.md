---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee20ce70a69b1ed68d003db980610fb00cecb845
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694994"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pinnedMessages = await graphClient.Chats["{chat-id}"].PinnedMessages
    .Request()
    .Expand("message")
    .GetAsync();

```