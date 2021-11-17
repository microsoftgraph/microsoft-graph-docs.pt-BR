---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97c7e31e9a874c40f4d23ef796e4663fe7bdfa1a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981703"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "name-value",
    ContentType = "contentType-value",
    IsInline = false,
    ContentLocation = "contentLocation-value",
    ContentBytes = Convert.FromBase64String("contentBytes-value")
};

await graphClient.Me.Messages["{message-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```