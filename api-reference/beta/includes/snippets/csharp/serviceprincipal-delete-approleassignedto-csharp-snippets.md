---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7abdb640a71db0a7f75261947064454f5fac40ef
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334025"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].AppRoleAssignedTo["{id}"]
    .Request()
    .DeleteAsync();

```