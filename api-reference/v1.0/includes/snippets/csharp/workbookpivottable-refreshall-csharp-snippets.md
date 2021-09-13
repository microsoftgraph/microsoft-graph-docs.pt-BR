---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc072796e9951f75a378ec0f88a592e8bc01dc201f2db247535f00f7cfa52536
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099923"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"].PivotTables
    .RefreshAll()
    .Request()
    .PostAsync();

```