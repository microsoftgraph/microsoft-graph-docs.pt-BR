---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4f115ec575f0a87f3366bc5b6541a990bbf6966
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038311"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chats = await graphClient.Users["{user-id}"].Chats
    .Request()
    .GetAsync();

```