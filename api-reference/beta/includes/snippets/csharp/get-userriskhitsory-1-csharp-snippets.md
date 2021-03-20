---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7daab6a0c652f22f7a450e4ccd80b09d13a211a6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953111"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var history = await graphClient.RiskyUsers["{riskyUser-id}"].History
    .Request()
    .GetAsync();

```