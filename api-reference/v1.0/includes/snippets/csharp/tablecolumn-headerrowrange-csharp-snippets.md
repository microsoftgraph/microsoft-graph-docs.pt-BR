---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26df2f4b4f8c0d735c9015837350cdf88787c4b8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609734"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .HeaderRowRange()
    .Request()
    .PostAsync();

```