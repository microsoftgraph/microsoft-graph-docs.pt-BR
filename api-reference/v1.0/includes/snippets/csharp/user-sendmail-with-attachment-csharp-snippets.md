---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 210ebe66a8bd6f1aa0863c4976e9fbdee084117e
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944709"
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
                Address = "meganb@contoso.onmicrosoft.com"
            }
        }
    },
    Attachments = new MessageAttachmentsCollectionPage()
    {
        new FileAttachment
        {
            Name = "attachment.txt",
            ContentType = "text/plain",
            ContentBytes = Encoding.ASCII.GetBytes("SGVsbG8gV29ybGQh")
        }
    }
};

await graphClient.Me
    .SendMail(message,null)
    .Request()
    .PostAsync();

```