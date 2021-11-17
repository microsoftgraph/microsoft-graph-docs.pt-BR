---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4cc439aa5ca5fc72e6e5092eb062a62f0d4a241f6148d55ea55e7d937d7f0376
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272297"
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