---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6159d4d227f4ca9add824fffa504de4b7cdf9f90
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130154"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columnDefinition = new ColumnDefinition
{
    Description = "test",
    EnforceUniqueValues = false,
    Hidden = false,
    Indexed = false,
    Name = "Title",
    Text = new TextColumn
    {
        AllowMultipleLines = false,
        AppendChangesToExistingText = false,
        LinesForEditing = 0,
        MaxLength = 255
    }
};

await graphClient.Sites["{site-id}"].Columns
    .Request()
    .AddAsync(columnDefinition);

```