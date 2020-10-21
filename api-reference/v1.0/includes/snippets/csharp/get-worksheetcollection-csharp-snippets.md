---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65bc190f85fab212ecdebf1f6aa3444f64c88588
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618726"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var worksheets = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets
    .Request()
    .GetAsync();

```