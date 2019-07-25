---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54da9e3a28a5338a749698a79a5d8b8d610ce080
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728968"
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