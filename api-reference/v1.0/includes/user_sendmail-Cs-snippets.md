---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 700bce7b4a331c6072582ddd9a8ca3c479decbf4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "Meet for lunch?",
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "The new cafeteria is open."
    },
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "fannyd@contoso.onmicrosoft.com"
            }
        }
    },
    CcRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "danas@contoso.onmicrosoft.com"
            }
        }
    }
};

var saveToSentItems = false;

await graphClient.Me
    .SendMail(message,saveToSentItems)
    .Request()
    .PostAsync();

```