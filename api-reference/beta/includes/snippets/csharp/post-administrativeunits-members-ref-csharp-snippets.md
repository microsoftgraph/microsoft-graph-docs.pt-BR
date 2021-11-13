---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64343e83446f1be3eada6b37c5d2cef56c96c52d
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890214"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.AdministrativeUnits["{administrativeUnit-id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```