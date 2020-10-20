---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5de63092708e0e499dfe378602fffa38d5250322
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611652"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Request()
    .Skip(5)
    .Top(5)
    .GetAsync();

```