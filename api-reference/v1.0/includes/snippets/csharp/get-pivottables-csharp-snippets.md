---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61a000e940e54d25f41306d16a8196150ada6551
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787722"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pivotTables = await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"].PivotTables
    .Request()
    .GetAsync();

```