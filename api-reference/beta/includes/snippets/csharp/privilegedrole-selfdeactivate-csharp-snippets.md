---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6e65b1da384ecf223b7b2746e8ef654846b748c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoles["{id}"]
    .SelfDeactivate()
    .Request()
    .PostAsync();

```