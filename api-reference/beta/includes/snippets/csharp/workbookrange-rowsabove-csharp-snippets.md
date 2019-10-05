---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e64df5f0cea804beb29e49e6432498f6464351fd
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402582"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsAbove(null)
    .Request()
    .PostAsync();

```