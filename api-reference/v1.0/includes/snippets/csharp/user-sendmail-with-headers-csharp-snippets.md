---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98db3f89c5ee7acf8c2eff230b0784fe3d73a05f
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2019
ms.locfileid: "37402919"
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
    .SendMail(message,null)
    .Request()
    .PostAsync();

```