---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7eb09350f6559355c9fd66370b53b8a278042f33
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684930"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "name-value",
    ContentType = "contentType-value",
    IsInline = false,
    ContentLocation = "contentLocation-value",
    ContentBytes = Encoding.ASCII.GetBytes("base64-contentBytes-value")
};

await graphClient.Me.Messages["{id}"].Attachments
    .Request()
    .AddAsync(attachment);

```