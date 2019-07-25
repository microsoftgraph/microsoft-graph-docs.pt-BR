---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5840f1dd77ac94c0b7bb4a26c56806d4938e327
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858159"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/beta/users/alexd@contoso.com"}
    }
};

await graphClient.Groups["{id}"].AcceptedSenders.References
    .Request()
    .AddAsync(directoryObject);

```