---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13efacc29d866a47b91df1bf968eb4ddd6c76252
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800417"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .Request()
    .GetAsync();

```