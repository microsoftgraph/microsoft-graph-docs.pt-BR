---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fac2e4a89cd4ab9b78a50d014fcad4ab2455121193ba0626ee54ce9ee7453b2a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275427"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChart = new WorkbookChart
{
    Id = "id-value",
    Height = 99,
    Left = 99
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts
    .Request()
    .AddAsync(workbookChart);

```