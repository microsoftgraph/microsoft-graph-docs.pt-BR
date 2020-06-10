---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03345d39c896ad8118171a1a4c53496012a44113
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683811"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Attachments = (IMessageAttachmentsCollectionPage)new List<Attachment>()
    {
        new FileAttachment
        {
            Name = "guidelines.txt",
            ContentBytes = Encoding.ASCII.GetBytes("bWFjIGFuZCBjaGVlc2UgdG9kYXk=")
        }
    }
};

var comment = "Please take a look at the attached guidelines before you decide on the name.";

await graphClient.Me.Messages["AAMkADA1MTAAAH5JaKAAA="]
    .ReplyAll(message,comment)
    .Request()
    .PostAsync();

```