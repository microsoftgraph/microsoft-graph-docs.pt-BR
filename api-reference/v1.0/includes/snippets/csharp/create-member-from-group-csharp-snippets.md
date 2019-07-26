---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 945d17bad66d7aeaa18892ede7a3995fbd4ba0c1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890071"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/v1.0/directoryObjects/{id}"}
    }
};

await graphClient.Groups["{id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```