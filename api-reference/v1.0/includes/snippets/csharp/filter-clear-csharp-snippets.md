---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7714f259d8c413627b1de87d4cfe61cb0aca9ca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779527"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns["{workbookTableColumn-id}"].Filter
    .Clear()
    .Request()
    .PostAsync();

```