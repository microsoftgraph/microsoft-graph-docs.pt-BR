---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3da8aa14f840d28ac87c467b149832fc6db45e0
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581585"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

Int32? index = null;

var values = JsonDocument.Parse("[[1,2,3],[4,5,6]]");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows
    .Add(index,values)
    .Request()
    .PostAsync();

```