---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1f5c98976264eff5f6a0ca36090d6693998fb565
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455338"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var toRecipients = new List<Recipient>()
{
    new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Name = "name-value",
            Address = "address-value"
        }
    }
};

await graphClient.Me.Messages["{id}"]
    .Forward(comment,toRecipients)
    .Request()
    .PostAsync();

```