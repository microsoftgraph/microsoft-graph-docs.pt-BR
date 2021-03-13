---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe90fb700f30951a4178cb63b49bcbd4b5cfc8da
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770082"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = await graphClient.Chats["{chat-id}"].Members["{conversationMember-id}"]
    .Request()
    .GetAsync();

```