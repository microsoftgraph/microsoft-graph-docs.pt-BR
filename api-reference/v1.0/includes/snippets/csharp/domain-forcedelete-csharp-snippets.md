---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0e5c597c2af5f5a78120a3b5bb2b51acbf97b411
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466369"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var disableUserAccounts = true;

await graphClient.Domains["{id}"]
    .ForceDelete(disableUserAccounts)
    .Request()
    .PostAsync();

```