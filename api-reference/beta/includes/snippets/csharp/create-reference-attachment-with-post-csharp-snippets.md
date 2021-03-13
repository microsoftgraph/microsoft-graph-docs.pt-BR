---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8da3d5003cfb1f193f36927c71c6237a994cc0a8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808405"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "I attached a reference to a file on OneDrive."
    },
    Attachments = new PostAttachmentsCollectionPage()
    {
        new ReferenceAttachment
        {
            Name = "Personal pictures",
            SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
            ProviderType = ReferenceAttachmentProvider.OneDriveConsumer,
            Permission = ReferenceAttachmentPermission.Edit,
            IsFolder = true
        }
    }
};

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"]
    .Reply(post)
    .Request()
    .PostAsync();

```