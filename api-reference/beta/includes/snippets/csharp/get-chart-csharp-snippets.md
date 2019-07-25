---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5553e6108c0cfdd0b5ebd5c03b01675bc889d4bb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708512"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChart = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"]
    .Request()
    .GetAsync();

```