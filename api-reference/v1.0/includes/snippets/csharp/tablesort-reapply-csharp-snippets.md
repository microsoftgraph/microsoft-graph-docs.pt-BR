---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 076fb649a4f0c7f27d40eff362ea6e773a343db0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804720"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Sort
    .Reapply()
    .Request()
    .PostAsync();

```