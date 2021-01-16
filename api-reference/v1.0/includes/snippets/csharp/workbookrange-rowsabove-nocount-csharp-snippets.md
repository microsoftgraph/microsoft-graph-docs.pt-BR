---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d18221ac5b5fabe2743550224d65d11b40b05b32
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882819"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsAbove()
    .Request()
    .GetAsync();

```