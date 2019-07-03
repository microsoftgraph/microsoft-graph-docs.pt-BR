---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5704ec2ca1657394506a10639334462ed458b7a9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492173"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Cell(5,6)
    .Request()
    .GetAsync();

```