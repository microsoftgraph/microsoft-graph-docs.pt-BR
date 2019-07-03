---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab8dd3fdcb386d6c07833cd97144c59f5144f2ba
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508589"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().EntireColumn()
    .Request()
    .GetAsync();

```