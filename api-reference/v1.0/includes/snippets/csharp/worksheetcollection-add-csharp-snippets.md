---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3a495bc94ddafdbddafd33f106c65c49410ea32d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608603"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var name = "name-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets
    .Add(name)
    .Request()
    .PostAsync();

```