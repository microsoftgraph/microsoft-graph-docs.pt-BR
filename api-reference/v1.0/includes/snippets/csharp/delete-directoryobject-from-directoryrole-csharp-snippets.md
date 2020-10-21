---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84c69da79d55b661e0791e650beb7868e7a570bc
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616821"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryRoles["{id}"].Members["{id}"].Reference
    .Request()
    .DeleteAsync();

```