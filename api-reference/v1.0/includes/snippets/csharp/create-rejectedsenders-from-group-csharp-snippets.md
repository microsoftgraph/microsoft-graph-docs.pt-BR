---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb5082b48bc1096ca4e8feba86f79f107f81cb70
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544134"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "alexd@contoso.com"
};

await graphClient.Groups["{id}"].RejectedSenders.References
    .Request()
    .AddAsync(directoryObject);

```