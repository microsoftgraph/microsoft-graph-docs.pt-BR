---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6710982af01bfc4f4c265ae8a00a7a9af2501cef6da80ef4ae500e1f62772f86
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899396"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Groups["{group-id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```