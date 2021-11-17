---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66cd5a7c805519a94b0ede93bb7208d4de9bdade
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004006"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "smile",
    ContentBytes = Convert.FromBase64String("R0lGODdhEAYEAA7")
};

await graphClient.Me.Messages["{message-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```