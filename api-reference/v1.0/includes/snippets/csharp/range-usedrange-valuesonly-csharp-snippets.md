---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa6e26d011a231f82ea41219c2134a11efd903d5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888577"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .UsedRange(true)
    .Request()
    .GetAsync();

```