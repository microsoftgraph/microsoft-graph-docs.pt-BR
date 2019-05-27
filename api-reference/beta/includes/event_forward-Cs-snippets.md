---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 085c6dc8a218713c3b9fa193f5e711986a3bf103
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436639"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ToRecipients = new List<Recipient>()
{
    new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Address = "danas@contoso.onmicrosoft.com",
            Name = "Dana Swope"
        }
    }
};

var Comment = "Dana, hope you can make this meeting.";

await graphClient.Me.Events["{id}"]
    .Forward(comment,toRecipients)
    .Request()
    .PostAsync();

```