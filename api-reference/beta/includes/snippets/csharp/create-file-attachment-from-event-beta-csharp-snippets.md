---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b90b32c619a8d3944109e0a9320899df48f8aacb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034485"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "menu.txt",
    ContentBytes = Convert.FromBase64String("bWFjIGFuZCBjaGVlc2UgdG9kYXk=")
};

await graphClient.Me.Events["{event-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```