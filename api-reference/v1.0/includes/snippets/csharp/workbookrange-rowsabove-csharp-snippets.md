---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48d7ce7dc83080a75c27d731c8e3884ec01c2e66
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882835"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsAbove(2)
    .Request()
    .GetAsync();

```