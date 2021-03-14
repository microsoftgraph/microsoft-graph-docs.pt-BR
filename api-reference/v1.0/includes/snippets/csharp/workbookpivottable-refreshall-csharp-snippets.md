---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93cd511fe73d57304fda3db9593c370decc2a346
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805290"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"].PivotTables
    .RefreshAll()
    .Request()
    .PostAsync();

```