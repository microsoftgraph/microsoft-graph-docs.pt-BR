---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 885184bcb43b978dd6108462fe69b0ab98ab7c49
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770039"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Me.Chats["{chat-id}"].Members
    .Request()
    .GetAsync();

```