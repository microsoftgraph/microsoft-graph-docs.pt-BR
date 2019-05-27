---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2bfd99aa7ac1df716af1f090afd3233f64043416
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435141"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var borders = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Borders
    .Request()
    .GetAsync();

```