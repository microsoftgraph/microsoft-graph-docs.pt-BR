---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54da9e3a28a5338a749698a79a5d8b8d610ce080
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478913"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    LastModifiedDateTime = "datetime-value",
    Name = "name-value",
    ContentType = "contentType-value",
    Size = 99,
    IsInline = true
};

await graphClient.Users["{id}"].Outlook.Tasks["{id}"].Attachments
    .Request()
    .AddAsync(attachment);

```