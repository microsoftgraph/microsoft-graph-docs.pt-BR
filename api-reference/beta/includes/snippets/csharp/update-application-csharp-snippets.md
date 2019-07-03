---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66b16f590e48ee5c9c9bce0b5f79174eae968390
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476258"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    AllowPublicClient = false,
    DisplayName = "New display name"
};

await graphClient.Applications["{id}"]
    .Request()
    .UpdateAsync(application);

```