---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47861edd08b7343e1e9cf6511a3d0c1f70c51d56
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889697"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rows = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range('A1:Z10')
    .VisibleView().Rows
    .Request()
    .GetAsync();

```