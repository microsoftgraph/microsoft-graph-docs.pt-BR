---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6603e74f1d7b75d74d1ec00e9f9483470315a8b1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714625"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsBefore(count)
    .Request()
    .PostAsync();

```