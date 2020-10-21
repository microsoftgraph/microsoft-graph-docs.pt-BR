---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19979e7c97b22748181f91c40244d0472c8c1e33
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603435"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rows = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows
    .Request()
    .GetAsync();

```