---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac0930e5beb9ceeb8de5b4843b7f3561f76f552c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805840"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookOperation = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Operations["{workbookOperation-id}"]
    .Request()
    .GetAsync();

```