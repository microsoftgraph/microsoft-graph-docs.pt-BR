---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd6b5889aa147b86ef28212376e6f94d16f9094f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944897"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tables = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Tables
    .Request()
    .GetAsync();

```