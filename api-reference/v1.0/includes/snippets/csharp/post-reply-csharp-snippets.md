---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6ac498defa637bc96fcbf276dcb1c7d422b536e2
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072357"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "content-value"
    },
    ReceivedDateTime = DateTimeOffset.Parse("datetime-value"),
    HasAttachments = true,
    From = new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Name = "name-value",
            Address = "address-value"
        }
    },
    Sender = new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Name = "name-value",
            Address = "address-value"
        }
    },
    ConversationThreadId = "conversationThreadId-value",
    NewParticipants = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Name = "name-value",
                Address = "address-value"
            }
        }
    },
    ConversationId = "conversationId-value",
    CreatedDateTime = DateTimeOffset.Parse("datetime-value"),
    LastModifiedDateTime = DateTimeOffset.Parse("datetime-value"),
    ChangeKey = "changeKey-value",
    Categories = new List<String>()
    {
        "categories-value"
    },
    Id = "id-value",
    InReplyTo = new Post
    {
    },
    Attachments = new PostAttachmentsCollectionPage()
    {
        new FileAttachment
        {
            LastModifiedDateTime = DateTimeOffset.Parse("datetime-value"),
            Name = "name-value",
            ContentType = "contentType-value",
            Size = 99,
            IsInline = true,
            Id = "id-value"
        }
    }
};

await graphClient.Groups["{id}"].Threads["{id}"].Posts["{id}"]
    .Reply(post)
    .Request()
    .PostAsync();

```