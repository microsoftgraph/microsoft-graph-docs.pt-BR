---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec016b4b22fedea790ce77abe4f1291d325a5983
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544124"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Attachments = new List<Attachment>()
    {
        new FileAttachment
        {
            Name = "guidelines.txt",
            ContentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
        }
    }
};

var comment = "Please take a look at the attached guidelines before you decide on the name.";

await graphClient.Me.Messages["AAMkADA1MTAAAH5JaKAAA="]
    .ReplyAll(message,comment)
    .Request()
    .PostAsync();

```