---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b364a19d648e3ae64dac573e774991e9e4cb3db9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466025"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().UsedRange(true)
    .Request()
    .GetAsync();

```