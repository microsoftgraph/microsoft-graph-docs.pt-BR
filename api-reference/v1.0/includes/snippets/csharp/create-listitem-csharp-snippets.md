---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2ce475a3f7582b880cbb32f87f01ae1cd5be5eea
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507920"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var listItem = new ListItem
{
    Fields = new FieldValueSet
    {
        Title = "Widget",
        Color = "Purple",
        Weight = 32
    }
};

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items
    .Request()
    .AddAsync(listItem);

```