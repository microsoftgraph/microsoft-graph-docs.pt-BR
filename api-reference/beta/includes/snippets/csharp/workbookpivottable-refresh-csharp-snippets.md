---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 557c138e2390f531e0022e0678669dae83a9a0cc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796112"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"].PivotTables["{workbookPivotTable-id}"]
    .Refresh()
    .Request()
    .PostAsync();

```