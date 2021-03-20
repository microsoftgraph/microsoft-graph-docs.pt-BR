---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9d8b5a7de8ab031a1bedc1b475a83b696e5bddd8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "0f933635-5b77-4cf4-a577-f78a5eb090a2"
};

await graphClient.DirectoryRoles["{directoryRole-id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```