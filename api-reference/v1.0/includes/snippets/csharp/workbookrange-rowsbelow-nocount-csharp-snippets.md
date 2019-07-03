---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9871f6b52e8cfd02f68d7b9fde19dcf034323d40
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507693"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"].Range().RowsBelow()
    .Request()
    .GetAsync();

```