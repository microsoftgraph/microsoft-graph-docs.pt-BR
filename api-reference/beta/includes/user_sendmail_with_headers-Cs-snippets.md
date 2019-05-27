---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ecbfd64fb26438641d658e14a6142eeee791e27
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455762"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "9/9/2018: concert",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "The group represents Nevada."
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
            Value = "Nevada"
        },
        new InternetMessageHeader
        {
            Name = "x-custom-header-group-id",
            Value = "NV001"
        }
    }
};

await graphClient.Me
    .SendMail(message,saveToSentItems)
    .Request()
    .PostAsync();

```