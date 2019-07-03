---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65bc190f85fab212ecdebf1f6aa3444f64c88588
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465565"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var worksheets = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets
    .Request()
    .GetAsync();

```