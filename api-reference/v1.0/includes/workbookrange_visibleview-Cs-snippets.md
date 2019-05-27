---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0e88817edda1e3781cfdbc0db36e0d3a0c34e3e5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454457"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeView = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"].Range('A1:Z10').VisibleView()
    .Request()
    .GetAsync();

```