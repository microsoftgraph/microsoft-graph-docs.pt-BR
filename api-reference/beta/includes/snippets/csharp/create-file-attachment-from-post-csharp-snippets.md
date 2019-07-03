---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bcdeee2ebe4e5e335b7cff9ebfe3f8d67ea66585
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463317"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    Name = "name-value",
    ContentBytes = "contentBytes-value"
};

await graphClient.Groups["{id}"].Threads["{id}"].Posts["{id}"].Attachments
    .Request()
    .AddAsync(attachment);

```