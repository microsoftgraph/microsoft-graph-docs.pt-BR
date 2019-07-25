---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2480e82825922c41a4fa4af8ef76493fe976093e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716031"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookWorksheet = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"]
    .Request()
    .GetAsync();

```