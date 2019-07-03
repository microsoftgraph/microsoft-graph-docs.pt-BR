---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30fab5a5f8f8f3e0016acc00f3f12c4e54c1d9eb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466358"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    Name = "menu.txt",
    ContentBytes = "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="
};

await graphClient.Me.Events["AAMkAGI1AAAt9AHjAAA="].Attachments
    .Request()
    .AddAsync(attachment);

```