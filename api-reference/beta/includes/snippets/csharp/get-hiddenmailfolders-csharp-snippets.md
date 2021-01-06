---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dcbb464efc9dc04f4cc594d3da1744f355641495
ms.sourcegitcommit: df0778a4dbd1e7a2fde1846bdfbfd9440fc91672
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("includeHiddenFolders", "true")
};

var mailFolders = await graphClient.Me.MailFolders
    .Request( queryOptions )
    .GetAsync();

```