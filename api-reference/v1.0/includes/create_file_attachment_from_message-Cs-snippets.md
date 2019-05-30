---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d2c0d544c87ccfc73c2bfc99d57eacc9fd69bc6
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546377"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    Name = "smile",
    ContentBytes = "base64R0lGODdhEAYEAA7"
};

await graphClient.Me.Messages["AAMkpsDRVK"].Attachments
    .Request()
    .AddAsync(attachment);

```