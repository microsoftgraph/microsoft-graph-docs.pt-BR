---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9441ffd5fab9721f76f5e0e5979d88f3b32ebe7f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns["{workbookTableColumn-id}"]
    .Range()
    .Request()
    .GetAsync();

```