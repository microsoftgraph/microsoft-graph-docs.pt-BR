---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35a95f4320b76fc65ee7f69836eb5f481421b09c867365fa31f5fce9191a3b7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159183"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .ColumnsAfter(2)
    .Request()
    .GetAsync();

```