---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88541e22a0196ab2307332702f01d606de0cb041
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622534"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows["{index}"]
    .Range()
    .Request()
    .PostAsync();

```