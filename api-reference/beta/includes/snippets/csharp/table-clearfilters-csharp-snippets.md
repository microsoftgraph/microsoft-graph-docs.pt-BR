---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92f51b551dd07a0e4804ecafa5785a08eb65eaca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .ClearFilters()
    .Request()
    .PostAsync();

```