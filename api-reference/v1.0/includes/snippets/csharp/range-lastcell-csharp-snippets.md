---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53c311b63425386faeec202eaa5324ade8e7f967
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466191"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().LastCell()
    .Request()
    .GetAsync();

```