---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e556f58b3208ec2bf0552c183ae054ef1ada3c81
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882956"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsBefore(2)
    .Request()
    .GetAsync();

```