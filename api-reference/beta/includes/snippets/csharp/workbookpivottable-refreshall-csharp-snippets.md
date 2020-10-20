---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7611f3f6de81fd57479c8e7044a5665e876dc097
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612159"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"].PivotTables
    .RefreshAll()
    .Request()
    .PostAsync();

```