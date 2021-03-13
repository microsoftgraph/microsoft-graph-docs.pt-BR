---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c83b276943bb290d75c3e6d5330930510cc7a0e7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Chats["{chat-id}"].Messages
    .Request()
    .GetAsync();

```