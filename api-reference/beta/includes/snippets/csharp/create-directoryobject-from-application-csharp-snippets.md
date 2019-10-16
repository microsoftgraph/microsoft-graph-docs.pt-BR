---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c355a577a5c6cc5010a61f2eea7b67a90daf644b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Applications["{id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```