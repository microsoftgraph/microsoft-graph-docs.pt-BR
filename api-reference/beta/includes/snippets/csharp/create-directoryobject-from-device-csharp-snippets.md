---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc8259d4f30f1075e640609b1cfbcf6eafd34843
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681071"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"directoryObject", "{}"}
    }
};

await graphClient.Devices["{id}"].RegisteredUsers.References
    .Request()
    .AddAsync(directoryObject);

```