---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43d38f1d850d13cf6c05fbeb6c3541b88185ea3c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775749"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chats = await graphClient.Users["{user-id}"].Chats
    .Request()
    .Expand("members")
    .GetAsync();

```