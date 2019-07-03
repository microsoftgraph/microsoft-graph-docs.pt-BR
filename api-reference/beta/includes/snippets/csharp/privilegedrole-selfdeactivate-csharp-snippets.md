---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6e65b1da384ecf223b7b2746e8ef654846b748c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518424"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoles["{id}"]
    .SelfDeactivate()
    .Request()
    .PostAsync();

```