---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b647d61ee1f4f358b94a0c3acab9a917c1ec56bc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805032"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Column(5)
    .Request()
    .GetAsync();

```