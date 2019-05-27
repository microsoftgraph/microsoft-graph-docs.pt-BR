---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b364a19d648e3ae64dac573e774991e9e4cb3db9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469822"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().UsedRange(true)
    .Request()
    .GetAsync();

```