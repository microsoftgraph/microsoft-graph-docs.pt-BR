---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc04092ab9760d7648b5104eface3bcda3d72454
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507520"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookWorksheetProtection = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Protection
    .Request()
    .GetAsync();

```