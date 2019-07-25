---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1a2039ff3ec1cc784ebc84df16a29e2c9bee7d6c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723647"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pivotTables = await graphClient.Drive.Root.Workbook.Worksheets["{id}"].PivotTables
    .Request()
    .GetAsync();

```