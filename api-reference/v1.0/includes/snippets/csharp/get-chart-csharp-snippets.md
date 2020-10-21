---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5553e6108c0cfdd0b5ebd5c03b01675bc889d4bb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChart = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"]
    .Request()
    .GetAsync();

```