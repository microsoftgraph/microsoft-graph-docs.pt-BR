---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1109d0b032d38cb7400ed5160f419dd4b98eed93
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477133"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var errors = await graphClient.Education.SynchronizationProfiles["{id}"].Errors
    .Request()
    .GetAsync();

```