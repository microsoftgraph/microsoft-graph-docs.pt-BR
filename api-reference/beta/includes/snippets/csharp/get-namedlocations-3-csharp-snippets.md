---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91a89294d4b0dd06b609edea6a16eafa5e009ab7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947403"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocations = await graphClient.Identity.ConditionalAccess.NamedLocations
    .Request()
    .Filter("createdDateTime ge 2019-09-01T00:00:00Z")
    .GetAsync();

```