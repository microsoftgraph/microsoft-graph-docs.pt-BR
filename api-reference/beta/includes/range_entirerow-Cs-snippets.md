---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2813b0a3fec9906b201c6722801373a2bad6154
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442911"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().EntireRow()
    .Request()
    .GetAsync();

```