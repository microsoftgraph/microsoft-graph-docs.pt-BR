---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f240c5ae590dbb01d2dcc0c1844409031dc72b40
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962706"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var names = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Names
    .Request()
    .GetAsync();

```