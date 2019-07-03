---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e21d42b603dc529118e69f0fce1ddafd59edd3e0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518421"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var my = await graphClient.PrivilegedRoleAssignments.My()
    .Request()
    .GetAsync();

```