---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89124d7cc56bd84f3f4085dbe7caaf34a18ec934
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466899"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Range('A1:B2')
    .Request()
    .GetAsync();

```