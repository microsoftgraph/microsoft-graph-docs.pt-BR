---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 885184bcb43b978dd6108462fe69b0ab98ab7c49
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254237"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Me.Chats["{chat-id}"].Members
    .Request()
    .GetAsync();

```