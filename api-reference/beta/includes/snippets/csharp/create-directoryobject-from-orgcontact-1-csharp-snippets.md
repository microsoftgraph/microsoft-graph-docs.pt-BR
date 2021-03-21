---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a843139b509efbd469be9f8b401461983ab74133
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957668"
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

await graphClient.Contacts["{orgContact-id}"].DirectReports
    .Request()
    .AddAsync(directoryObject);

```