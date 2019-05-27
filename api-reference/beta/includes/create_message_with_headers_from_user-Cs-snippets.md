---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 979cdb95e2ca624079bf71bd5072c54809c1c344
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440223"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "9/8/2018: concert",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "The group represents Washington."
    },
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "AlexW@contoso.OnMicrosoft.com"
            }
        }
    },
    InternetMessageHeaders = new List<InternetMessageHeader>()
    {
        new InternetMessageHeader
        {
            Name = "x-custom-header-group-name",
            Value = "Washington"
        },
        new InternetMessageHeader
        {
            Name = "x-custom-header-group-id",
            Value = "WA001"
        }
    }
};

await graphClient.Me.Messages
    .Request()
    .AddAsync(message);

```