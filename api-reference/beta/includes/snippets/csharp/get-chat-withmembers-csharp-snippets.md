---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00f171ccfb9702c05118c4c8fee6e670ef60a37ae6cff1437b2ad72925231d6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899973"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = await graphClient.Chats["{chat-id}"]
    .Request()
    .Expand("members")
    .GetAsync();

```