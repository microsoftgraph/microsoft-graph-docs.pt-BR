---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53a16c2d449251903a3902f3575f54c16a5564b0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793718"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"].PivotTables
    .RefreshAll()
    .Request()
    .PostAsync();

```