---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f8cf0b5352f99f2cf3b701ed3face7fca3591b1
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617110"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var series = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Series
    .Request()
    .GetAsync();

```