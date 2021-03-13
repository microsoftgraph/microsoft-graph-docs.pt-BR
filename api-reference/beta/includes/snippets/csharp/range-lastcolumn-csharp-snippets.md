---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50c192cb9e11a47e5b78b954cc8514b2b56448ec
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798140"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .LastColumn()
    .Request()
    .GetAsync();

```