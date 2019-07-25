---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0dc71b6cb192b5faef6296aed191ea9590a3cab5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706995"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registeredUsers = await graphClient.Devices["{id}"].RegisteredUsers
    .Request()
    .GetAsync();

```