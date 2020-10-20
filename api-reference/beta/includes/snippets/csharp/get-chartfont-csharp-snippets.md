---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3e6420d528d7058fd95327db1afb7faf0f9f3e4c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartFont = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis.Format.Font
    .Request()
    .GetAsync();

```