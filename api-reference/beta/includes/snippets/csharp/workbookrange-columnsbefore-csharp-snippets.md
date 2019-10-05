---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1f69bf37253bcb2cc9a3c9923636b4aa083c320
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402575"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsBefore(null)
    .Request()
    .PostAsync();

```