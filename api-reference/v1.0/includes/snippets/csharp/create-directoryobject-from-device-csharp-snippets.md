---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 633d6a815a0a17c4aaea840978d55fc291343486
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680798"
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

await graphClient.Devices["{id}"].RegisteredUsers
    .Request()
    .AddAsync(directoryObject);

```