---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf75e8a209455c550995ee2a368e954744afa94d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775721"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chats = await graphClient.Users["{user-id}"].Chats
    .Request()
    .Filter("members/any(o: o/displayname eq 'Peter Parker')")
    .Expand("members")
    .GetAsync();

```