---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f24070b15b0eb3195301cd3c666439c0074109a5
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522643"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{user-id}"
};

await graphClient.DirectoryRoles["{role-objectId}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```