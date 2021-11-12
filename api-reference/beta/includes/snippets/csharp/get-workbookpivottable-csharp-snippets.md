---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85b38ee34175a129dcb180069be8aa6e82379804ebd981234976834024c3a78a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101446"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookPivotTable = await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"].PivotTables["{workbookPivotTable-id}"]
    .Request()
    .GetAsync();

```