---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 655078525861be01928d1587d24dc81132aa3658d017ab577fde4e8acc5b1cfc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102540"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = await graphClient.Users["{user-id}"].Chats["{chat-id}"]
    .Request()
    .GetAsync();

```