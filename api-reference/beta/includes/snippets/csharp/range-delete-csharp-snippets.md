---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20a18b4fb0e9d25b67b552b8c6277b66d79171a9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477129"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = "shift-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Delete(shift)
    .Request()
    .PostAsync();

```