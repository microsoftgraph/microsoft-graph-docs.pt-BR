---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 051fc235f5c9121a75a07cf1f95093660825322e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeSort = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Sort
    .Request()
    .GetAsync();

```