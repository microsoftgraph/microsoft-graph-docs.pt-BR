---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcfa10a6b7dfc32a2055fa544697e5b58a0f134b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .ColumnsAfter(2)
    .Request()
    .GetAsync();

```