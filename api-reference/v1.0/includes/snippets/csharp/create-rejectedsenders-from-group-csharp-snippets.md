---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5622ca15d3dd1e859351a79c762162167a3ecae8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806119"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "alexd@contoso.com"
};

await graphClient.Groups["{group-id}"].RejectedSenders.References
    .Request()
    .AddAsync(directoryObject);

```