---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 054336833d11d1d6e5ac5cfadb5a55f2dc4b6b7b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookNamedItem = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Request()
    .GetAsync();

```