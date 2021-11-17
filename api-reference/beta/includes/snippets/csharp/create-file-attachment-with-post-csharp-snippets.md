---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8add9a5cbee1c45342738a2d185cb97dac0036af505f7b52b53fc34ad7fccb6b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272295"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "Which quarter does that file cover? See my attachment."
    },
    Attachments = new PostAttachmentsCollectionPage()
    {
        new FileAttachment
        {
            Name = "Another file as attachment",
            ContentBytes = Encoding.ASCII.GetBytes("VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu")
        }
    }
};

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"]
    .Reply(post)
    .Request()
    .PostAsync();

```