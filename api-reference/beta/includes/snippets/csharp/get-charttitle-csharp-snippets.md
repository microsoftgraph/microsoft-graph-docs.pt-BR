---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe240f739a2484aaa5ff728f0dc99bebea6c982d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615198"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartTitle = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Title
    .Request()
    .GetAsync();

```