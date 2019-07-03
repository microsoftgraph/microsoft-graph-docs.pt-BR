---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb45e3738300a3171aa2cbd81ec8dfab3cded157
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507635"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Font
    .Request()
    .GetAsync();

```