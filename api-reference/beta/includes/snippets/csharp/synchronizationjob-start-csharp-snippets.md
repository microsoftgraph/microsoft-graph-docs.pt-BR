---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2478b99008a79a75d8b5fdee81c53561ff908f44
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498819"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"]
    .Start()
    .Request()
    .PostAsync();

```