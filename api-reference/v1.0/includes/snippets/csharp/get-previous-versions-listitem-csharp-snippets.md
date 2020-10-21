---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83d4bcb292d0a4020675fc40c82d8485a781a6a3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604209"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var versions = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"].Versions
    .Request()
    .GetAsync();

```