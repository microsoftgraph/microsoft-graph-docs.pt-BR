---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce3e8ce6e6b0e914e740c03bacf16ef4f977cc41
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775896"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Chats["{chat-id}"].Members["{conversationMember-id}"]
    .Request()
    .DeleteAsync();

```