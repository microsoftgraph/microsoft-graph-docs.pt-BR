---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9fa85464b632686053f4b95901e37e29948946f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466733"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Range()
    .Request()
    .GetAsync();

```