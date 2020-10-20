---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a30ec7733186ae4cd6c83ff0ebf4a842862c96cc
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615502"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .ReapplyFilters()
    .Request()
    .PostAsync();

```