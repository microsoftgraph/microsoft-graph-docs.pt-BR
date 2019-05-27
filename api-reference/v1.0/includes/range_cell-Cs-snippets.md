---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5704ec2ca1657394506a10639334462ed458b7a9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452781"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Cell(5,6)
    .Request()
    .GetAsync();

```