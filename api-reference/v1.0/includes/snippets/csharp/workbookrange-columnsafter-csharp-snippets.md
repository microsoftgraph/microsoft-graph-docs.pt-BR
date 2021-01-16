---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06c3a41b3b163fa2176e06c5cbae8f47c02bae36
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883137"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsAfter(2)
    .Request()
    .GetAsync();

```